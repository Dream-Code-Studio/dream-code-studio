<script>
  export let title;
  export let items;
</script>

<ul class="list">
  <h4 class="title">{title}</h4>
  {#each items as item}
    <li class="item">{item}</li>
  {/each}
</ul>

<style>
  .list {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .title {
    font-family: "Bebas Neue", sans-serif;
    font-weight: 400;
    font-size: 24px;
  }
  .item {
    list-style: none;
    font-family: 'Satoshi-Regular';
    font-size: 20px;
  }
</style>
