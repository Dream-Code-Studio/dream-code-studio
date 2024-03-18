<script>
  export let title;
  export let highlight;
  export let src;
</script>

<div class="card">
  <div class="title">{title}</div>
  <div class="info">
    {#each highlight as item}
      <div class="item">{item}</div>
    {/each}
  </div>
  <div
    class="img"
    style:background-image={`url(${src})`}
    style:background-size={"cover"}
  ></div>
</div>

<style>
  .card {
    position: relative;
    border: 2px solid #514955;
    display: inline-block;
    padding: 48px;
    border-radius: 12px;
    overflow: hidden;
  }
  .img {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    opacity: 0;
    transition: opacity 0.3s ease-in-out;
  }
  .card:hover .img{
    opacity: 1;
  }
  .title {
    font-family: "Satoshi-black";
    font-size: 60px;
    text-align: center;
    color: black;
    margin-bottom: 72px;
    text-shadow:
      -1px -1px 0 #f6e3ff,
      1px -1px 0 #f6e3ff,
      -1px 1px 0 #f6e3ff,
      1px 1px 0 #f6e3ff;
  }
  .card:hover .title {
    color: #f6e3ff;
    text-shadow: none;
  }
  .info {
    font-family: "Satoshi-Regular";
    font-size: 20px;
    color: #f6e3ff;
  }
</style>
