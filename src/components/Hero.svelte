<script>
  import cal from "../assets/cal.jpg";
  import callum from "../assets/callum.jpg";

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

<!-- <div id="heroWrapper">
  <div class="intro">
    <h1>CALLUM LAING</h1>
    <p class="subtitle">Front-End Developer in England, UK.</p>
  </div>
</div> -->

<div class="heroContainer">
  <div class="aboutHero">
    <p>
      I'm a front-end developer based in the UK, passionate about creating
      dynamic, user-friendly websites. With the same drive and teamwork I bring
      to American football and rugby, I build sleek, responsive interfaces that
      perform just as well under pressure. Let's connect and tackle new
      challenges together!
    </p>

    <p>
      It's an exciting journey, and since recently retiring from many years of
      playing Rugby and American Football, it's been fulfilling redirecting that
      energy and passion into Web Development.
    </p>
    <h1>Callum Laing</h1>
  </div>
  <div class="imgHero">
    <img class="cal" src={cal} alt="" />
    <img class="callum" src={callum} alt="" />
  </div>
</div>

<style>
  .heroContainer {
    display: grid;
    place-items: center;
    grid-template-columns: 1fr 1fr;
    padding: 13em;
  }

  .imgHero {
    --box-size: 100px;
    display: inline-grid;
    padding-right: calc(var(--box-size) / 2);
    padding-bottom: calc(var(--box-size) / 2);
    & > * {
      grid-area: 1 / 1;
    }
  }

  .imgHero > img {
    width: calc(var(--box-size) * 4);
    height: calc(var(--box-size) * 4);
    border: 1px solid black;
    box-shadow: 2px 2px 2px;
  }

  .cal {
    transform: translateX(70%);
    background-color: rgba(230, 232, 232);
  }
  .callum {
    transform: translateY(50%);
    background-color: rgba(230, 232, 232);
  }

  h1 {
    font-size: 4em;
    margin: 0;
    font-family: "Herr Von Muellerhoff", cursive;
    font-weight: 400;
    font-style: normal;
  }

  p {
    font-size: 1.4rem;
    font-family: "Cormorant Garamond", serif;
    font-weight: 500;
    font-style: normal;
  }

  a {
    text-decoration: none;
    color: black;
    margin-top: 25px;
  }

  @media (max-width: 768px) {
  }

  @media (min-width: 768px) and (max-width: 1024px) {
  }
</style>
