<script>
  export let title;
  export let highlight;
</script>

<div class="card">
  <div class="title">{title}</div>
  <div class="info">
    {#each highlight as item}
      <div class="item">{item}</div>
    {/each}
  </div>
</div>

<style>
  .card {
    border: 2px solid #514955;
    display: inline-block;
    padding: 48px;
    border-radius: 12px;
  }
  .title {
    font-family: "Satoshi-black";
    font-size: 60px;
    text-align: center;
    color: black;
    margin-bottom: 72px;
    text-shadow:
      -1px -1px 0 #F6E3FF,
      1px -1px 0 #F6E3FF,
      -1px 1px 0 #F6E3FF,
      1px 1px 0 #F6E3FF;
  }
  .info {
    font-family: 'Satoshi-Regular';
    font-size: 20px;
    color: #F6E3FF;
  }
</style>
