<script>
  import Background from "./Background.svelte";
  import Button from "../../components/Button.svelte";
</script>

<div class="home">
  <div class="content">
    <div class="title">
      Coding Creativity
      <br />
      Into Reality
    </div>
    <div class="subtitle">
      We make all of your digital dreams a reality lorem ipsum dolor sit amet
    </div>
    <Button text="Contact Us" />
  </div>
  <Background />
</div>
<img class="ribbons" src="/Ribbons.png" alt="">

<style>
  .home {
    max-width: 1200px;
    margin: auto;
    position: relative;
  }
  .content {
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .title {
    font-size: 68px;
    color: #f9edff;
    font-family: "Satoshi-Black";
    margin-bottom: 12px;
  }
  .subtitle {
    font-size: 16px;
    color: #b4b4b4;
    font-family: "Satoshi-Regular";
    width: 400px;
    margin: auto;
    margin-bottom: 28px;
  }
  .ribbons {
    display: block;
    width: 100%;
    max-width: 1200px;
    margin: auto;
    padding-bottom: 60px;
  }
</style>
