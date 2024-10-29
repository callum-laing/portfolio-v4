<script>
  function scrollToElement(event) {
    event.preventDefault();
    const targetId = event.target.getAttribute("href").substring(1);
    const targetElement = document.getElementById(targetId);
    if (targetElement) {
      targetElement.scrollIntoView({
        behavior: "smooth",
        block: "start",
      });
    }
  }
</script>

<section class="hero">
  <h1>Callum Laing</h1>
  <nav>
    <a href="">Projects</a>
    <a href="">About</a>
    <a href="">Contact</a>
  </nav>
</section>

<style>
  .hero {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: 100dvh;
    background: linear-gradient(
      to bottom,
      rgb(26, 25, 25) 0%,
      rgb(26, 25, 25) 15%,
      rgb(181, 125, 125) 50%,
      rgb(181, 125, 125) 50%,
      rgb(26, 25, 25) 85%
    );
    padding-bottom: 100px;
  }

  h1 {
    font-size: 8rem;
    font-family: "Kaushan Script", cursive;
    font-weight: 400;
    font-style: normal;
    color: black;
    text-shadow:
      -1px -1px 0 rgba(255, 255, 255, 0.2),
      1px -1px 0 rgba(255, 255, 255, 0.2),
      -1px 1px 0 rgba(255, 255, 255, 0.2),
      1px 1px 0 rgba(255, 255, 255, 0.2);
  }

  nav {
    display: flex;
    justify-content: center;
    width: 60%;
  }

  nav a {
    font-size: 2rem;
    margin: 0 20px;
    text-decoration: none;
    color: black;
    font-family: "Inknut Antiqua", serif;
    font-weight: 300;
    font-style: normal;
    line-height: 1;
    transition:
      font-weight 1s eaase,
      color 0.3s ease;
  }
  nav a:hover {
    font-weight: bold;
  }
</style>
