<script>
  import hero from "$lib/images/hero.svg";
</script>

<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200&icon_names=arrow_outward"
/>
<section class="hero">
  <div class="hero-text">
    <h1>Tech Problems <span>- Simplified<span>.</span></span></h1>
    <p>From web development, computer repairs, technical trainings, and more</p>
    <div class="btn-container">
      <a href="/" class="neo-btn primary"
        >Explore Services <span class="material-symbols-outlined">
          arrow_outward
        </span>
      </a>
    </div>
  </div>
  <div class="hero-img neo-container hover">
    <img src={hero} alt="" />
    <!-- <img src="https://avatar.iran.liara.run/public/job/operator/male" alt="" /> -->
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
    font-weight: var(--fw-normal);
    display: flex;
    flex-direction: column;
  }

  h1 span {
    color: var(--primary);
    font-size: calc(var(--fs-h1) - 5px);
    font-weight: var(--fw-bold);
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

  .material-symbols-outlined {
    font-variation-settings:
      "FILL" 0,
      "wght" 300,
      "GRAD" 0,
      "opsz" 40;
  }
</style>
