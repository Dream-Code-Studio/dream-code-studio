<script>
  import Background from "./Background.svelte";
  import Button from "../../components/Button.svelte";
</script>

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
<div class="background"><Background /></div>

<style>
  .content {
    text-align: center;
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
