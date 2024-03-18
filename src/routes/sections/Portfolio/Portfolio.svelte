<script>
  import PortfolioCard from "./components/PortfolioCard.svelte";
  const cards = [
    {
      title: "Interiorlicious",
      highlight: ["React", "Svelte", "Vue"],
    },
    {
      title: "Portfolio",
      highlight: ["React", "Svelte", "Vue"],
    },
    {
      title: "E-commerce",
      highlight: ["React", "Svelte", "Vue"],
    },
    {
      title: "Portfolio",
      highlight: ["React", "Svelte", "Vue"],
    },
  ];
</script>

<div class="portfolio">
  <div class="title">Portfolio</div>
  <div class="cards">
    {#each cards as card}
    <PortfolioCard title={card.title} highlight={card.highlight} />
  {/each}
  </div>
</div>

<style>
  .portfolio {
    margin-top: 120px;
  }
  .title {
    font-family: 'Satoshi-Bold';
    font-size: 48px;
    text-align: center;
    color: white;
    margin-bottom: 40px;
  }
  .cards {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 32px;
  }
</style>
