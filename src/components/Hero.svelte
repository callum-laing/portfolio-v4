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
    padding-top: 75px;
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

  .button-74 {
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    background-color: rgba(214, 144, 24);
    border: 2px solid #422800;
    border-radius: 10px;
    color: black;
    cursor: pointer;
    display: inline-block;
    font-weight: 600;
    font-size: 18px;
    padding: 0 18px;
    line-height: 50px;
    text-align: center;
    text-decoration: none;
    user-select: none;
    -webkit-user-select: none;
    touch-action: manipulation;
  }

  .button-74:hover {
    background-color: white;
    box-shadow: none;
  }

  .button-74:active {
    box-shadow: #422800 2px 2px 0 0;
    transform: translate(2px, 2px);
  }

  @media (min-width: 768px) {
    .button-74 {
      min-width: 120px;
      padding: 0 25px;
    }
  }

  @media (max-width: 768px) {
    #heroWrapper {
      padding-top: 100px;
      padding-bottom: 200px;
    }
    .intro {
      height: 100%;
      width: auto;
      text-align: center;
      padding-right: 0;
    }
    h1 {
      font-size: 3.5rem;
    }
    .subtitle {
      font-size: 1rem;
      margin-top: 10px;
    }
    img {
      display: none;
    }
    a {
      margin-top: 50px;
    }
  }

  @media (min-width: 769px) and (max-width: 1024px) {
  }
</style>
