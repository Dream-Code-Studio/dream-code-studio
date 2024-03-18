<script>
  import Home from "./sections/Home/Home.svelte";
  import Portfolio from "./sections/Portfolio/Portfolio.svelte";
  import CTA from "./sections/CTA/CTA.svelte";
</script>

<section id="home" class="home">
  <Home/>
</section>
<section id="portfolio" class="home">
  <Portfolio/>
</section>
<section id="cta" class="home">
  <CTA/>
</section>


<style>
  :global(body) {
    background-color: rgba(3, 0, 9, 1);
  }
  .home {
    margin-top: 120px;
  }
  
</style>
