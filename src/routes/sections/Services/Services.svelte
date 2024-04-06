<script>
  import Background from "../Home/Background.svelte";
  import Button from "../../components/Button.svelte";
</script>

<div class="services-section">
  <div class="content">
    <div class="small-text">GET IN TOUCH</div>
    <div class="big-text">
      <div class="text">LET’S GET</div>
      <div class="outline">STARTED</div>
    </div>
    <Button text="Contact Us" />
  </div>
  <Background />
</div>

<style>
  .services-section {
    position: relative;
    text-align: center;
    line-height: 72px;
    padding-block: 80px;
    width: 90%;
    margin: auto;
    max-width: 1200px;
  }
  .content {
    z-index: 1;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
  }
  .small-text {
    font-size: 16px;
    color: #f2d6ff;
    font-family: "Satoshi-Regular";
  }
  .big-text {
    font-size: 68px;
    font-family: "Satoshi-Black";
    margin-bottom: 28px;
  }
  .text {
    color: #f9edff;
  }
  .outline {
    color: black;
    text-shadow:
      -1px -1px 0 #d164d3,
      1px -1px 0 #d164d3,
      -1px 1px 0 #d164d3,
      1px 1px 0 #d164d3;
  }
  @media (width < 700px) {
    .big-text {
      font-size: 52px;
    }
  }
  @media (width < 550px) {
    .small-text {
      font: 12px;
    }
    .big-text {
      font-size: 40px;
      line-height: 52px;
    }
  }
</style>
