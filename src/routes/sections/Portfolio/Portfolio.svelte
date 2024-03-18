<script>
  import PortfolioCard from "./components/PortfolioCard.svelte";
  const cards = [
    {
      title: "Interiorlicious",
      highlight: ["React", "Svelte", "Vue"],
      src: '/Card1.png'
    },
    {
      title: "Portfolio",
      highlight: ["React", "Svelte", "Vue"],
      src: '/Card2.png'
    },
    {
      title: "E-commerce",
      highlight: ["React", "Svelte", "Vue"],
      src: '/Card3.png'
    },
    {
      title: "Portfolio",
      highlight: ["React", "Svelte", "Vue"],
      src: '/Card4.png'
    },
  ];
</script>

<div class="portfolio">
  <div class="title">Portfolio</div>
  <div class="cards">
    {#each cards as card}
    <PortfolioCard title={card.title} highlight={card.highlight} src={card.src} />
  {/each}
  </div>
</div>

<style>
  .portfolio {
    margin-top: 180px;
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
