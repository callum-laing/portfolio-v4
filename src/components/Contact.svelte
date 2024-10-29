<script>
</script>

<div id="contactContainer">
  <h2>Contact</h2>
  <form action="https://formspree.io/f/xknykdjb" method="POST">
    <label for="name">
      <p class="formHeader">Your Name:</p>
      <input
        type="text"
        name="name"
        placeholder="What should I call you?"
        required
      />
    </label>
    <label for="email">
      <p class="formHeader">Your Email:</p>
      <input
        type="email"
        name="email"
        placeholder="What is your email?"
        required
      />
    </label>
    <label for="message">
      <p class="formHeader">Message:</p>
      <textarea
        rows="8"
        name="message"
        class="body"
        placeholder="Please leave your message here..."
        required
      ></textarea>
    </label>
    <button class="formSubmit" type="submit">Submit</button>
  </form>
</div>

<style>
  #contactContainer {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: 100vh;
    background: linear-gradient(
      to bottom,
      rgb(26, 25, 25) 0%,
      rgb(181, 125, 125) 50%,
      rgb(26, 25, 25) 100%
    );
    padding: 2em 1em;
    color: #fff;
    text-align: center;
  }

  h2 {
    font-size: 5rem;
    margin-bottom: 1em;
  }

  form {
    display: flex;
    flex-direction: column;
    gap: 15px;
    width: 90%;
    max-width: 600px;
  }

  label {
    display: flex;
    flex-direction: column;
    font-weight: 500;
  }

  input,
  textarea {
    border: 2px solid rgba(255, 255, 255, 0.2);
    padding: 10px;
    background-color: rgba(0, 0, 20);
    color: #ccd0e8;
    border-radius: 3px;
    font-size: 1em;
    font-family: "Roboto", sans-serif;
  }

  textarea {
    resize: vertical; /* Allows the user to resize vertically */
  }

  input:focus,
  textarea:focus {
    outline: none;
    border-color: #ccc;
  }

  button.formSubmit {
    padding: 10px;
    border: none;
    border-radius: 3px;
    background-color: rgba(181, 125, 125);
    color: #fff;
    font-size: 1em;
    cursor: pointer;
    transition: background-color 0.3s;
  }

  button.formSubmit:hover {
    background-color: rgba(255, 255, 255, 0.2);
  }

  @media (min-width: 768px) {
    h2 {
      font-size: 4.5rem;
    }

    form {
      width: 80%;
    }

    input {
      height: 40px;
      margin-top: 5px;
    }
  }
</style>
