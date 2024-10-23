<script>
  import html from "../assets/svg/html.svg";
  import css from "../assets/svg/css.svg";
  import javascript from "../assets/svg/javascript.svg";
  import react from "../assets/svg/react.svg";
  import svelte from "../assets/svg/svelte.svg";
</script>

<h1>Contact</h1>
<div id="contactContainer">
  <div class="extra-info">
    <div class="skillIcons">
      <img src={html} alt="html icon" width="50" height="auto" loading="lazy" />
      <span>HTML5</span>
    </div>
    <div class="skillIcons">
      <img src={css} alt="css icon" width="50" height="auto" loading="lazy" />
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
  <div class="contact-form">
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
      <button class="formSubmit" type="submit">Submit</button>
    </form>
  </div>
</div>

<style>
  #contactContainer {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }

  h1 {
    font-size: 5em;
    margin: 0;
    text-align: center;
    text-decoration-line: underline;
    text-decoration-color: black;
    text-underline-offset: 0.05em;
    text-decoration-thickness: 5px;
    margin-bottom: 1em;
    font-family: "Cormorant Garamond", serif;
    font-weight: bold;
    font-style: normal;
  }

  form {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  input,
  textarea {
    width: 600px;
    height: 30px;
    border: 2px solid rgba(255, 255, 255, 0.2);
    padding: 5px;
    background-color: rgba(0 0, 20);
    color: #ccd0e8;
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    font-size: 0.9em;
    border-radius: 3px;
  }

  @media (max-width: 768px) {
  }

  @media (min-width: 769px) and (max-width: 1024px) {
  }
</style>
