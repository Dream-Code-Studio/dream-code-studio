<script>
  const navbar = ["Home", "Projects", "Services", "Contact"];
  let navIndex = 1;
  let gap = 12;
  function handleClick(index) {
    navIndex = index;
    console.log(navIndex);
  }
</script>

<nav class="navbar" style:--gap={gap} style:--index={navIndex}>
  <div class="links">
    {#each navbar as item, index}
      <a class="link" on:click={() => handleClick(index)}>{item}</a>
    {/each}
    <div class="light"></div>
    <div class="active-link">Home</div>
  </div>
</nav>
<slot />

<style>
  .navbar {
    position: absolute;
    top: 0;
    left: 0;
    display: inline-block;
    background-color: rgb(6, 1, 28, .7);
    border-radius: 100px;
    border: 1px solid rgb(66, 0, 97.7);
    margin-top: 20px;
  }
  .links {
    display: inline-flex;
    gap: calc(var(--gap) * 1px);
    position: relative;
    margin: 12px;
  }
  .link {
    padding: 12px;
    border-radius: 100px;
    width: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: sans-serif;
    color: #F7E6FF;
    z-index: 2;
    cursor: default;
  }
  .active-link {
    width: 80px;
    padding: 12px;
    border-radius: 100px;
    background-color: #160020;
    position: absolute;
    top: 0;
    left: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: sans-serif;
    transition: 0.6s all ease-in-out;
    color: transparent;
    transform: translate(calc(var(--index) * (100% + var(--gap) * 1px)), 0);
  }
  .light {
    background-color: white;
    width: 80px;
    margin: 0 12px;
    height: 1px;
    position: absolute;
    top: calc(-13px - 1px);
    transition: 0.6s all ease-in-out;
    transform: translate(calc(var(--index) * (100% + 24px + var(--gap) * 1px)), 0);
    left: 0;
    box-shadow: 0 2px 12px 0 white;
  }
</style>
