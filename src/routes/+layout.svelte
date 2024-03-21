<script>
  import Navbar from "./components/Navbar.svelte";
  import Logo from "./components/Logo.svelte";
  import Button from "./components/Button.svelte";
  import { onMount } from "svelte";

  let scrolled = false;

  onMount(()=> {
    window.addEventListener('scroll', ()=> {
      scrolled = window.scrollY > 0 ? true : false;
    })
  })
</script>

<div class="wrapper">
  <header class={`header ${scrolled && 'scrolled'}`}>
    <Logo />
    <Navbar />
    <Button text="Hire Us" />
  </header>
  <slot />
</div>

<style>
  .wrapper {
    max-width: 1200px;
    margin: auto;
    position: relative;
  }
  .scrolled  {
    background-color: white;
  }
  .header {
    position: sticky;
    margin: auto;
    top: 32px;
    left: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    z-index: 2;
  }
</style>
