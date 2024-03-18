<script>
  import Button from "./components/Button.svelte";
  import Background from "./components/Background.svelte";
</script>

<section id="home" class="home">
  <div class="content">
    <div class="title">
      Coding Creativity
      <br>
      Into Reality
    </div>
    <div class="subtitle">
      We make all of your digital dreams a reality lorem ipsum dolor sit amet
    </div>
    <Button text="Contact Us" />
  </div>
  <div class="background"><Background /></div>
</section>

<style>
  :global(body) {
    background-color: rgba(3, 0, 9, 1);
  }
  .home {
    height: 100vh;
    margin-top: 120px;
  }
  .content {
    text-align: center;
  }
  .title {
    font-size: 68px;
    color: #F9EDFF;
    font-family: 'Satoshi-Black';
    margin-bottom: 12px;
  }
  .subtitle {
    font-size: 16px;
    color: #B4B4B4;
    font-family: 'Satoshi-Regular';
    width: 300px;
    margin: auto;
    margin-bottom: 28px;
  }
  .background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100px;
    z-index: -1;
  }
</style>
