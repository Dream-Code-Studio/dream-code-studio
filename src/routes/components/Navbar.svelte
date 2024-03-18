<script>
  const navbar = ["Home", "Projects", "Services", "Contact"];
  let navIndex = 0;
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

<style>
  .navbar {
    background-color: rgb(6, 1, 28, 0.7);
    border-radius: 100px;
    border: 1px solid rgb(66, 0, 97.7);
    display: inline-block;
  }

  .links {
    display: inline-flex;
    gap: calc(var(--gap) * 1px);
    margin: 12px;
    position: relative;
  }

  .link {
    align-items: center;
    border-radius: 100px;
    color: #f7e6ff;
    cursor: default;
    display: flex;
    font-family: sans-serif;
    justify-content: center;
    padding: 12px;
    width: 80px;
    z-index: 2;
  }

  .active-link {
    align-items: center;
    background-color: #160020;
    border-radius: 100px;
    color: transparent;
    display: flex;
    font-family: sans-serif;
    justify-content: center;
    left: 0;
    padding: 12px;
    position: absolute;
    top: 0;
    transform: translate(calc(var(--index) * (100% + var(--gap) * 1px)), 0);
    transition: 0.6s all ease-in-out;
    width: 80px;
  }

  .light {
    background-color: white;
    box-shadow: 0 2px 12px 0 white;
    height: 1px;
    left: 0;
    margin: 0 12px;
    position: absolute;
    top: calc(-13px - 1px);
    transform: translate(
      calc(var(--index) * (100% + 24px + var(--gap) * 1px)),
      0
    );
    transition: 0.6s transform ease-in-out;
    width: 80px;
  }
</style>
