<script>
</script>

<svelte:head>
  <title>Home | Zebra ICT Centre</title>
  <meta name="description" content="Zebra ICT Centre" />
</svelte:head>
<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0&icon_names=arrow_right_alt"
/>
<section class="hero">
  <div class="hero-text">
    <h1>Tech Problems <span>- Simplified<span>.</span></span></h1>
    <p>From web development, computer repairs, technical trainings, and more</p>
    <div class="btn-container">
      <a href="/" class="neo-btn primary"
        >Explore Services <span class="material-symbols-outlined">
          arrow_right_alt
        </span>
      </a>
    </div>
  </div>
  <div class="hero-img neo-container hover">
    <img src="https://avatar.iran.liara.run/public/job/operator/male" alt="" />
  </div>
</section>

<style>
  .hero {
    display: flex;
    justify-content: space-between;
    align-items: start;
    flex: 1;
  }

  .hero-text {
    display: flex;
    flex-direction: column;
    align-items: start;
    gap: var(--space-sm);
    width: min(100%, 500px);
  }

  h1 {
    font-family: var(--heading-font);
    font-size: var(--fs-h2);
    display: flex;
    flex-direction: column;
  }

  h1 span {
    color: var(--primary);
    font-size: calc(var(--fs-h1) - 5px);
  }
  h1 span span {
    color: var(--text);
  }

  P {
    font-size: calc(var(--fs-h3) - 3px);
  }

  .btn-container {
    display: flex;
    gap: var(--space-md);
    flex-wrap: wrap;
    align-items: center;
    justify-content: left;
    padding: var(--space-md) 0;
  }
  a {
    font-size: var(--fs-h4);
    background: var(--primary);
    color: var(--highlight);
  }

  a span {
    font-size: 25px;
    color: inherit;
  }

  .hero-img {
    width: min(100%, 500px);
    overflow: hidden;
    padding: var(--space-md);
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .hero-img img {
    width: 100%;
  }

  @media screen and (max-width: 768px) {
    .hero {
      flex-direction: column;
    }
  }
</style>
