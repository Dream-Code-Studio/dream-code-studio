<script>
  import Button from "./components/Button.svelte";
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
    font-size: 100px;
    color: #F9EDFF;
    font-family: 'Satoshi-Black';
  }
  .subtitle {
    font-size: 24px;
    color: #B4B4B4;
    font-family: 'Satoshi-Regular';
    width: 500px;
    margin: auto;
  }
</style>
