<script>
  import Navbar from "./components/Navbar.svelte";
  import Logo from "./components/Logo.svelte";
  import Button from "./components/Button.svelte";
  import { onMount } from "svelte";

  let scrolled = false;

  onMount(() => {
    window.addEventListener("scroll", () => {
      scrolled = window.scrollY > 0 ? true : false;
    });
  });
</script>

<div class={`header-wrapper ${scrolled && "scrolled"}`}>
  <header class="header">
    <Logo />
    <Navbar />
    <Button text="Hire Us" />
  </header>
</div>
<slot />

<style>
  .wrapper {
    max-width: 1200px;
    margin: auto;
    position: relative;
  }
  .scrolled {
    backdrop-filter: blur(12px);
    /* background-color: white; */
    box-shadow: 0 10px 10px 0 rgba(0, 0, 0, 0.3);
  }
  .header-wrapper {
    position: relative;
    position: sticky;
    top: 0;
    left: 0;
    z-index: 10;
  }
  .header {
    max-width: 1200px;
    margin: auto;
    padding-block: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }
</style>
