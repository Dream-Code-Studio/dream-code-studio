<script>
  import Background from "../Home/Background.svelte";
  import Button from "../../components/Button.svelte";
</script>

<div class="services-section">
  <div class="content">
    <div class="small-text">GET IN TOUCH</div>
    <div class="text">LET’S GET <br /><span class="outline">STARTED</span></div>
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
  }
  .content {
    z-index: 1;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .small-text {
    font-size: 16px;
    color: #f2d6ff;
    font-family: "Satoshi-Regular";
  }
  .text {
    font-size: 68px;
    color: #f9edff;
    font-family: "Satoshi-Black";
    margin-bottom: 28px;
  }
  .outline {
    color: black;
    text-shadow:
      -1px -1px 0 #d164d3,
      1px -1px 0 #d164d3,
      -1px 1px 0 #d164d3,
      1px 1px 0 #d164d3;
  }
</style>
