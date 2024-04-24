<div id="contactContainer">
  <h1 class="contact">Get in touch</h1>
  <!-- <p class="txt">Feel free to leave me a message; I try to reply to everyone when I'm able to. Please don't spam.</p> -->
  <div class="grid-wrap">
    <form action="https://formspree.io/f/xknykdjb" method="POST">
      <label for="subject">
        <p>Your name:</p>
        <input
          type="text"
          name="subject"
          placeholder="What should I call you?"
        />
      </label>
      <label for="email">
        <p>Your email:</p>
        <input type="email" name="subject" placeholder="What is your email?" />
      </label>
      <label for="body">
        <p>Message:</p>
        <textarea
          rows="5"
          name="body"
          class="body"
          placeholder="Please leave your message here..."
        />
      </label>
      <button class="button-74" type="submit">Send</button>
    </form>
  </div>
</div>

<style>
  #contactContainer {
    padding-left: 50px;
    padding-right: 50px;
    padding-top: 150px;
    padding-bottom: 100px;
  }

  .grid-wrap {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
  p {
    color: white;
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
    color: rgba(200, 255, 200);
  }

  ::placeholder {
    color: rgba(237, 232, 187);
  }
  h1 {
    margin-bottom: 0;
  }

  p {
    color: white;
    font-size: 1.1em;
  }
  form {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  .button-74 {
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
    font-family: verdana;
    font-size: 0.9em;
    border-radius: 10px;
  }

  .body {
    width: 600px;
    height: 150px;
    resize: none;
  }

  @media (max-width: 769px) {
    .grid-wrap {
      display: flex;
      flex-direction: column;
      margin-bottom: 50px;
      gap: 10px;
    }
    input,
    textarea,
    .body {
      width: 275px;
      height: auto;
      margin: 0 auto;
    }
    h1 {
      font-size: 2rem;
    }
    p {
      width: 100%;
      margin: 0;
    }
    .txt {
      padding-bottom: 10px;
      font-size: 1em;
    }
  }

  @media (min-width: 770px) and (max-width: 1024px) {
    input,
    textarea {
      width: 600px;
    }
    p {
      width: 100%;
    }
  }
</style>
