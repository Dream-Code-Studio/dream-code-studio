<script>
  import Navbar from "./components/Navbar.svelte";
  import Logo from "./components/Logo.svelte";
  import Button from "./components/Button.svelte";
</script>

<div class="wrapper">
  <header class="header">
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
  .header {
    position: absolute;
    margin: auto;
    top: 0;
    left: 0;
    display: flex;
    justify-content: space-between;
    width: 100%;
    margin: 20px;
  }
</style>
