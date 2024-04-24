<div class="hireContainer">
  <div class="aboutContainer">
    <div class="aboutMe">
      <h1>Who am I?</h1>
      <p>
        I'm a Front-End Developer with a background in sales administration and
        a passion for coding. By day, I'm immersed in the world of sales
        operations, where I thrive on ensuring seamless processes and supporting
        the sales team.
      </p>
      <p>
        Outside of work, I'm a sports enthusiast and enjoy playing American
        football at the highest level in the UK. Hiking with my partner and our
        dog, typically in the Scottish Highlands, is another favourite hobby of
        mine, allowing me to unwind and take in the breath-taking scenery.
      </p>
    </div>
  </div>
  <div class="formContainer">
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
          <input
            type="email"
            name="subject"
            placeholder="What is your email?"
          />
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
</div>

<style>
  .hireContainer {
    display: flex;
    justify-content: center;
    align-items: center;
    /* backdrop-filter: blur(20px);
    background: rgba(255, 255, 255, 0.07);
    border-radius: 8px;
    border: 2px solid rgba(255, 255, 255, 0.3); */
  }
  .aboutContainer {
    width: 40%;
  }
</style>
