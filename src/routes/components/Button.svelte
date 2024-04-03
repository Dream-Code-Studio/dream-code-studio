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
    margin: 4px;
    padding: 20px 24px;
    border-radius: 100px;
    font-size: 16px;
    font-family: "Satoshi-Bold";
  }
</style>