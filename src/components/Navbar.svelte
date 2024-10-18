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
    <a class="alink" href="#contactLink" on:click={scrollToElement}>Contact</a>
  </div>
</nav>

<style>
  nav {
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
    padding-bottom: 15px;
    padding-top: 15px;
    position: fixed;
    width: 100%;
    z-index: 1000;
    background-color: rgba(0, 10, 30);
  }

  a {
    text-decoration: none;
    font-size: 1.2em;
    /* color: rgba(200, 255, 200); */
    color: rgba(237, 232, 187);
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    margin: 0 10px;
  }

  a:hover {
    text-decoration-line: underline;
    text-decoration-color: rgba(50, 250, 250, 0.7);
    text-underline-offset: 0.15em;
    text-decoration-thickness: 0.2em;
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
