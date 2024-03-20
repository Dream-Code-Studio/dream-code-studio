<script>
  import Home from "./sections/Home/Home.svelte";
  import Portfolio from "./sections/Portfolio/Portfolio.svelte";
  import CTA from "./sections/CTA/CTA.svelte";
  import Footer from "./sections/Footer/Footer.svelte";
</script>

<section id="home" class="home">
  <Home/>
</section>
<section id="portfolio" class="portfolio">
  <Portfolio/>
</section>
<section id="cta" class="cta">
  <CTA/>
</section>
<section id="footer" class="footer">
  <Footer/>
</section>


<style>
  :global(body) {
    background-color: rgba(3, 0, 9, 1);
  }
  .home {
    margin-top: 120px;
  }
  
</style>
