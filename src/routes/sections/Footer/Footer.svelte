<script>
  import List from "./components/List.svelte";
  import Logo from "../../components/Logo.svelte";
  import Facebook from "./components/Facebook.svelte";
  import Twitter from "./components/Twitter.svelte";
  import Instagram from "./components/Instagram.svelte";
  import LinkedIn from "./components/LinkedIn.svelte";

  const footerData = {
    Members: ["Ethan", "Valerian", "Warren"],
    Company: ["About", "Contact"],
    "Learn More": ["Comunity", "Blog", "FAQ"],
  };
</script>

<div class="wrapper">
  <div class="footer">
    <div class="upper-section">
      <div class="logo"><Logo /></div>
      {#each Object.keys(footerData) as title}
        <div class="list">
          <List {title} items={footerData[title]} />
        </div>
      {/each}
    </div>
    <div class="divider"></div>
    <div class="lower-section">
      <div class="copyright">© 2024 DreamCodeStudios. All rights reserved.</div>
      <div class="links">
        <div class="link"><Facebook /></div>
        <div class="link"><Twitter /></div>
        <div class="link"><Instagram /></div>
        <div class="link"><LinkedIn /></div>
      </div>
    </div>
  </div>
</div>

<style>
  .wrapper {
    position: relative;
    background: linear-gradient(90deg, #140018, #14021f, #0a0113);
  }
  .footer {
    max-width: 1200px;
    color: white;
    margin: auto;
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .upper-section {
    display: flex;
    justify-content: space-between;
    padding: 80px 0;
  }
  .divider {
    width: 100%;
    height: 2px;
    background-color: #432C4E;
  }
  .list,
  .logo {
    flex: 1;
  }
  .lower-section {
    display: flex;
    justify-content: space-between;
    padding: 20px;
  }
  .copyright {
    font-family: "Satoshi-Regular";
    font-size: 24px;
  }
  .links {
    display: flex;
    gap: 20px;
  }
</style>
