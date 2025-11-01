<script>
  export let items = [];
</script>

<div class="marquee-container">
  <div class="marquee">
    {#each items as item}
      <span class="marquee-item">{item}</span>
    {/each}
  </div>

  <div class="marquee marquee2">
    {#each items as item}
      <span class="marquee-item">{item}</span>
    {/each}
  </div>
</div>

<style>
  .marquee-container {
    position: relative;
    width: 100%;
    overflow-x: hidden;
    border-top: 2px solid var(--text);
    border-bottom: 2px solid var(--text);
  }

  .marquee {
    display: inline-block;
    white-space: nowrap;
    padding: var(--space-md) 0;
    animation: marquee 15s linear infinite;
  }

  .marquee2 {
    position: absolute;
    top: 0;
    left: 0;
    animation: marquee2 15s linear infinite;
  }

  .marquee-item {
    margin: 0 var(--space-md);
    font-size: var(--fs-h3);
    font-family: var(--heading-font);
  }

  @keyframes marquee {
    0% {
      transform: translateX(0%);
    }
    100% {
      transform: translateX(-100%);
    }
  }

  @keyframes marquee2 {
    0% {
      transform: translateX(100%);
    }
    100% {
      transform: translateX(0%);
    }
  }
</style>
