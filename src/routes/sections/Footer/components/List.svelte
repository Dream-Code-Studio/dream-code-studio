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
    align-items: center;
    gap: 24px;
  }
  .title {
    font-family: "Bebas Neue", sans-serif;
    font-weight: 400;
    font-size: 24px;
    color: #F9EDFF;
  }
  .item {
    list-style: none;
    font-family: 'Satoshi-Regular';
    font-size: 20px;
  }
  @media (width < 650px) {
    .list {
      gap: 8px;
    }
  }
  @media (width < 500px) {
    .title {
      font-size: 20px;
    }
    .item {
      font-size: 16px;
    }
  }
</style>
