<script>
  import html from "../assets/svg/html.svg";
  import css from "../assets/svg/css.svg";
  import javascript from "../assets/svg/javascript.svg";
  import react from "../assets/svg/react.svg";
  import svelte from "../assets/svg/svelte.svg";
</script>

<div id="contactContainer">
  <div class="aboutContainer">
    <div class="aboutMe contact">
      <h1>About Me.</h1>
      <p>
        I'm a <span class="highlight">Front-End Developer</span> with a background
        in sales administration and a passion for coding. By day, I'm immersed in
        the world of sales operations, where I thrive on ensuring seamless processes
        and supporting the sales team.
      </p>
      <p>
        Outside of work, I'm a sports enthusiast and enjoy playing American
        football at the highest level in the UK. Hiking with my partner and our
        dog, typically in the Scottish Highlands, is another favourite hobby of
        mine, allowing me to unwind and take in the breath-taking scenery.
      </p>
      <div class="skillsContainer">
        <div class="skillIcons">
          <img
            src={html}
            alt="html icon"
            width="50"
            height="auto"
            loading="lazy"
          />
          <span>HTML5</span>
        </div>
        <div class="skillIcons">
          <img
            src={css}
            alt="css icon"
            width="50"
            height="auto"
            loading="lazy"
          />
          <span>CSS3</span>
        </div>
        <div class="skillIcons">
          <img
            src={javascript}
            alt="javascript icon"
            width="50"
            height="auto"
            loading="lazy"
          />
          <span>JavaScript</span>
        </div>
        <div class="skillIcons">
          <img
            src={svelte}
            alt="svelte icon"
            width="50"
            height="auto"
            loading="lazy"
          />
          <span>Svelte</span>
        </div>
        <div class="skillIcons">
          <img
            src={react}
            alt="react icon"
            width="50"
            height="auto"
            loading="lazy"
          />
          <span>React</span>
        </div>
      </div>
    </div>
  </div>

  <div class="grid-wrap">
    <h1>Let's chat.</h1>
    <form action="https://formspree.io/f/xknykdjb" method="POST">
      <label for="subject">
        <p class="formHeader">Your name:</p>
        <input
          type="text"
          name="subject"
          placeholder="What should I call you?"
          required
        />
      </label>
      <label for="email">
        <p class="formHeader">Your email:</p>
        <input
          type="email"
          name="subject"
          placeholder="What is your email?"
          required
        />
      </label>
      <label for="body">
        <p class="formHeader">Message:</p>
        <textarea
          rows="5"
          name="body"
          class="body"
          placeholder="Please leave your message here..."
          required
        />
      </label>
      <button class="button-74" type="submit">Send</button>
    </form>
  </div>
</div>

<style>
  #contactContainer {
    display: flex;
    padding-left: 50px;
    padding-right: 50px;
    padding-top: 150px;
    padding-bottom: 100px;
  }

  .aboutContainer {
    width: 50%;
    margin-right: 50px;
  }

  .skillsContainer {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    align-items: center;
    margin-bottom: 100px;
    padding-block: 50px;
    gap: 20px;
  }

  .skillIcons {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 10px;
    padding: 10px;
  }

  span {
    color: white;
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  .highlight {
    font-size: 1.2rem;
    font-weight: bold;
    color: rgba(237, 232, 187);
    font-style: normal;
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  a {
    text-decoration: none;
    color: rgba(237, 232, 187);
  }

  p {
    color: white;
    font-size: 1.1em;
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    max-width: 80ch;
  }

  h1 {
    font-size: 4em;
    margin: 0;
    display: inline-block;
    background-image: linear-gradient(
      to right,
      rgba(237, 232, 187),
      rgba(237, 232, 187)
    );
    background-size: 100% 2px;
    background-position: bottom;
    background-repeat: no-repeat;
    margin-bottom: 25px;
  }

  ::placeholder {
    color: rgba(237, 232, 187);
  }

  form {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  .formHeader {
    padding-top: 20px;
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

  input,
  textarea {
    width: 600px;
    height: 30px;
    border: 2px solid rgba(255, 255, 255, 0.5);
    padding: 5px;
    background-color: #1d2242;
    color: #ccd0e8;
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    font-size: 0.9em;
    border-radius: 10px;
  }

  .formHeader {
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    margin: 0;
  }

  .body {
    width: 600px;
    height: auto;
    resize: none;
  }

  @media (max-width: 768px) {
    #contactContainer {
      align-items: center;
      flex-direction: column;
    }
    input,
    textarea,
    .body {
      width: 275px;
      height: auto;
      margin: 0 auto;
    }
    /* h1 {
      font-size: 2rem;
    } */
    p {
      width: 100%;
      margin-bottom: 10px;
    }
    .skillsContainer {
      display: none;
    }
    .aboutContainer {
      width: 100%;
      margin: 0;
      padding-bottom: 25px;
    }
    .formHeader {
      padding-top: 20px;
    }
  }

  @media (min-width: 769px) and (max-width: 1024px) {
    #contactContainer {
      flex-wrap: wrap;
      padding-right: 0;
    }
    .aboutContainer {
      width: 100%;
      padding-bottom: 25px;
    }
    input,
    textarea {
      width: 600px;
    }
    p {
      max-width: 70ch;
    }
    .skillsContainer {
      display: none;
    }
    .formHeader {
      padding-top: 20px;
    }
  }
</style>
