<script>
  import Home from "./sections/Home/Home.svelte";
  import Portfolio from "./sections/Portfolio/Portfolio.svelte";
  import Services from "./sections/Services/Services.svelte";
  import Footer from "./sections/Footer/Footer.svelte";
</script>

<section id="home" class="home">
  <Home/>
</section>
<section id="portfolio" class="portfolio">
  <Portfolio/>
</section>
<section id="services" class="services">
  <Services/>
</section>
<section id="footer" class="footer">
  <Footer/>
</section>


<style>
  :global(body) {
    background-color: rgba(3, 0, 9, 1);
  }
  .home {
    margin-top: 80px;
  }
  
</style>
