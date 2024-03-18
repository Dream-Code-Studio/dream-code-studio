<script>
  import Home from "./sections/Home/Home.svelte";
  import Portfolio from "./sections/Portfolio/Portfolio.svelte";
  import CTA from "./sections/CTA/CTA.svelte";
</script>

<section id="home" class="home">
  <Home/>
  <Portfolio/>
  <CTA/>
</section>

<style>
  :global(body) {
    background-color: rgba(3, 0, 9, 1);
  }
  .home {
    height: 100vh;
    margin-top: 120px;
  }
  
</style>
