<script>
  import calfootie from "../assets/contactImages/calfootie.png";

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

<div id="heroWrapper">
  <div class="intro">
    <h1>CALLUM LAING</h1>
    <p class="subtitle">Front-End Developer in England, UK.</p>
  </div>
  <img class="calImg" src={calfootie} alt="" />
</div>

<style>
  #heroWrapper {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    padding-top: 200px;
    padding-bottom: 250px;
  }

  .intro {
    font-size: 3rem;
    width: 40%;
    padding-right: 20px;
    padding-top: 150px;
  }

  h1 {
    font-size: 8rem;
    margin: 0;
  }

  .subtitle {
    font-size: 0.5em;
    font-weight: 400;
    color: rgba(237, 232, 187);
    margin: 0;
  }

  img {
    width: auto;
    height: 500px;
  }

  a {
    text-decoration: none;
    color: black;
    margin-top: 25px;
  }

  p {
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  @media (max-width: 768px) {
    #heroWrapper {
      display: grid;
      height: 100dvh;
      margin: 0;
      padding: 0;
    }

    .intro {
      width: 100%;
      text-align: center;
      padding: 0;
      margin-top: 100px;
    }

    h1 {
      font-size: 4rem;
      text-align: center;
    }
    .subtitle {
      font-size: 1.3rem;
    }
    img {
      opacity: 25%;
      height: 400px;
    }

    a {
      margin-top: 50px;
    }
  }

  @media (min-width: 769px) and (max-width: 1024px) {
    #heroWrapper {
      height: 100;
    }
  }
</style>
