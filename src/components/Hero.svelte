<script>
</script>

<section class="hero">
  <h1>Callum Laing</h1>
  <nav>
    <a href="#projects">Projects</a>
    <a href="#aboutSection">About</a>
    <a href="#contactContainer">Contact</a>
  </nav>
</section>

<style>
  .hero {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: 100vh;
    padding-bottom: 100px;

    background: linear-gradient(
      to bottom,
      rgb(26, 25, 25) 0%,
      rgb(26, 25, 25) 15%,
      rgb(81, 139, 179) 50%,
      rgb(81, 139, 179) 50%,
      rgb(26, 25, 25) 85%
    );
  }

  h1 {
    font-size: 8rem;
    font-family: "Kaushan Script", cursive;
    font-weight: 400;
    color: black;
    text-shadow:
      -1px -1px 0 rgba(255, 255, 255, 0.2),
      1px -1px 0 rgba(255, 255, 255, 0.2),
      -1px 1px 0 rgba(255, 255, 255, 0.2),
      1px 1px 0 rgba(255, 255, 255, 0.2);
    line-height: 1.2;
  }

  nav {
    display: flex;
    justify-content: center;
    width: 60%;
  }

  nav a {
    position: relative;
    font-size: 2rem;
    margin: 0 30px;
    text-decoration: none;
    color: black;
    font-family: "Montserrat", sans-serif;
    transition: color 0.3s ease;
  }

  nav a::after {
    content: "";
    position: absolute;
    left: 50%;
    bottom: -5px;
    width: 0;
    height: 5px;
    background-color: rgb(200, 200, 200);
    transition:
      width 0.3s ease,
      left 0.3s ease;
  }

  nav a:hover {
    color: rgba(0, 0, 0, 0.8);
  }

  nav a:hover::after {
    width: 100%;
    left: 0;
  }

  @media (max-width: 1024px) {
    h1 {
      font-size: 6rem;
    }

    nav a {
      font-size: 1.5rem;
      margin: 0 15px;
    }
  }

  @media (max-width: 768px) {
    h1 {
      font-size: 4rem;
      margin: 0 auto;
    }

    nav a {
      font-size: 1.2rem;
      margin: 0 10px;
    }
  }
</style>
