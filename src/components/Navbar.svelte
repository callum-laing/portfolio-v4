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

<nav>
  <div class="links">
    <a class="alink" href="#heroWrapper" on:click={scrollToElement}>Home</a>
    <a class="alink" href="#projects" on:click={scrollToElement}>Projects</a>
    <a class="alink" href="#contactContainer" on:click={scrollToElement}
      >About</a
    >
  </div>
</nav>

<style>
  nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding-bottom: 15px;
    padding-top: 15px;
    backdrop-filter: blur(20px);
    background: rgba(255, 255, 255, 0.07);
    position: fixed;
    width: 100%;
    z-index: 1000;
  }

  a {
    text-decoration: none;
    margin-left: 20px;
    font-size: 1.2em;
    color: rgba(200, 255, 200);
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  a:hover {
    border-bottom: 2px solid rgba(237, 232, 187);
  }

  .links {
    letter-spacing: 2px;
  }

  @media (max-width: 768px) {
    nav {
      display: flex;
      justify-content: space-around;
    }
    h1 {
      display: none;
    }
    a {
      font-size: 0.8em;
    }
  }
</style>
