<script>
  import shopPicture from "$lib/images/tech-user.png";
  import Hero from "$lib/components/Hero.svelte";
  import Marquee from "$lib/components/Marquee.svelte";
  const labels = [
    "Web Development",
    "Computer Repair",
    "Trainings",
    "Graphic Designing",
    "Mobile Accessories",
  ];
</script>

<svelte:head>
  <title>Home | Zebra ICT Centre</title>
  <meta name="description" content="Zebra ICT Centre" />
</svelte:head>

<Hero />
<section>
  <Marquee items={labels} />
</section>

<section>
  <div class="card neo-container hover">
    <img src="https://avatar.iran.liara.run/public/job/operator/male" alt="" />
    <div>
      <h2>Get computer knowledge</h2>
      <p>
        Learn how to use computers and be productive with them. Get technical
        trainings to repair both hardware and software of phones and computers.
      </p>
      <a href="/">Discovers courses</a>
    </div>
  </div>
  <div class="card neo-container hover">
    <img src={shopPicture} alt="" />
    <div>
      <h2>Get low prices</h2>
      <p>
        Browse our vast caterlog of tech products and find the one that best
        fits your needs. From laptops to mobile phones, we have it all.
      </p>
      <a href="/">Explore our collection</a>
    </div>
  </div>
</section>

<style>
  section {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .card {
    display: flex;
    align-items: center;
    gap: var(--space-md);
    width: 48%;
  }
  .card img {
    width: 170px;
  }

  .card div {
    display: flex;
    flex-direction: column;
    gap: var(--space-md);
  }

  .card h2,
  .card p,
  .card a {
    color: var(--text-dark);
  }

  .card div h2 {
    font-size: var(--fs-h4);
  }

  .card a {
    text-decoration: underline;
  }

  .card:first-child {
    background: var(--success);
  }

  .card:nth-child(2) {
    background: var(--info);
  }

  @media screen and (max-width: 768px) {
    section {
      flex-direction: column;
      gap: var(--space-lg);
    }
    .card {
      width: 100%;
      flex-direction: column;
    }
    .card img {
      height: 250px;
      object-fit: contain;
      object-position: c;
    }
  }
</style>
