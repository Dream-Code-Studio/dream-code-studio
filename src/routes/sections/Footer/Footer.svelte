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

<div class="footer">
  <div class="upper-section">
    <div class="logo"><Logo /></div>
    {#each Object.entries(footerData) as [title, items]}
      <div class="list">
        <List {title} items={footerData[title]} />
      </div>
    {/each}
  </div>
  <div class="divider"></div>
  <div class="bottom-section">
    <div class="copyright">© 2024 DreamCodeStudios. All rights reserved.</div>
    <div class="links">
      <div class="link"><Facebook /></div>
      <div class="link"><Twitter /></div>
      <div class="link"><Instagram /></div>
      <div class="link"><LinkedIn /></div>
    </div>
  </div>
  <div class="violet circle"></div>
  <div class="purple circle"></div>
  <div class="red circle"></div>
  <div class="blue circle"></div>
  <div class="glassmorphism"></div>
</div>

<style>
  .footer {
    color: white;
    display: flex;
    flex-direction: column;
    gap: 20px;
    position: relative;
    backdrop-filter: blur(10px);
  }
  .upper-section {
    display: flex;
    justify-content: space-between;
  }
  .divider {
    width: 100%;
    height: 2px;
    background-color: rgb(66, 66, 66);
  }
  .list,
  .logo {
    flex: 1;
    text-align: center;
  }
  .bottom-section {
    display: flex;
    justify-content: space-between;
  }
  .copyright {
    font-family: "Satoshi-Regular";
  }
  .links {
    display: flex;
    gap: 20px;
  }
  .purple {
    background-color: #6a0080;
  }
  .red {
    background-color: #a40027;
  }
  .blue {
    background-color: #29009d;
  }
  .violet {
    background-color: #5d0059;
  }
  .circle {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    position: absolute;
    top: 0;
    left: 0;
  }
  .glassmorphism {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background-color: rgb(187, 187, 187, 0.4);
    backdrop-filter: blur(1000px);
  }
</style>
