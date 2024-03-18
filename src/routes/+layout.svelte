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
    position: sticky;
    margin: auto;
    top: 32px;
    left: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }
</style>
