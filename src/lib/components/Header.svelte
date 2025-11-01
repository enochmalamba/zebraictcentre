<script>
  import logo from "../images/logo.png";
</script>

<header>
  <div class="logo">
    <img src={logo} alt="Zebra ICT Centre logo" />
  </div>
  <nav>
    <ul>
      <li><a href="/">Services</a></li>
      <li><a href="/">Portfolio</a></li>
      <li><a href="/">Shop</a></li>
      <li><a href="/">About</a></li>
      <li><a href="/">Contact</a></li>
    </ul>
  </nav>
  <div>
    <button title="Toggle Menu" class="menu-toggle"
      ><i class="bx bx-menu-wider"></i></button
    >
  </div>
</header>

<style>
  header {
    display: flex;
    align-items: center;
    padding: var(--space-sm) var(--space-md);
    background: var(--bg-light);
    margin: var(--space-lg) auto;
    width: fit-content;
    gap: var(--space-lg);
    border-radius: var(--radius-lg);
    border-bottom: 5px solid var(--border);
  }

  .logo img {
    height: 50px;
    border-radius: var(--radius-md);
  }

  ul {
    list-style: none;
    display: flex;
    align-items: center;
    gap: var(--space-md);
  }

  li a {
    font-size: var(--fs-base);
  }
  div {
    display: flex;
    align-items: center;
    gap: var(--space-md);
  }

  button {
    all: unset;
    padding: var(--space-xs);
    display: flex;
    align-items: center;
    justify-content: center;
    background: var(--bg-primary);
    border-radius: var(--radius-md);
    cursor: pointer;
    display: none;
  }

  button i {
    font-size: 28px;
  }
</style>
