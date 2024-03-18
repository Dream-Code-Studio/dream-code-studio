<script>
  export let text;
</script>

<button on:click class="btn">
  {text}
</button>

<style>
  .btn {
    border: none;
    outline: none;
    min-width: 140px;
    background-color: #E8B7FF;
    padding: 12px;
    margin: 4px;
    border-radius: 100px;
    font-size: 18px;
  }
</style>