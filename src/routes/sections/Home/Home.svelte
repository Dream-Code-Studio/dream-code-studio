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
  <div class="background">
    <Background />
  </div>
</div>
<div class="img">
  <img class="ribbons" src="/Ribbons.png" alt="" />
</div>

<style>
  .home {
    max-width: 1200px;
    width: 90%;
    height: 600px;
    margin: auto;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .content {
    text-align: center;

    width: 100%;
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
  .background {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
    height: 100%;
    z-index: -1;
  }
  .img {
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
  }
  @media (width < 1100px) {
    .home {
      height: 500px;
    }
  }
  @media (width < 800px) {
    .home {
      height: 400px;
    }
    .title {
      font-size: 52px;
    }
    .subtitle {
      width: 300px;
    }
  }
  @media (width < 500px) {
    .home {
      height: 300px;
    }
    .title {
      font-size: 40px;
    }
    .subtitle {
      width: 250px;
      font-size: 14px;
    }
  }
  @media (width < 400px) {
    .ribbons {
      width: 600px;
    }
  }
  @media (width < 400px) {
    .home {
      height: 350px;
    }
  }
</style>
