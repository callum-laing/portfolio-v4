<script>
  import github from "../assets/svg/github.svg";
  import linkedin from "../assets/svg/linkedin.svg";
</script>

<main>
  <div class="footer">
    <div class="links">
      <span class="linkIcon"
        ><a href="https://github.com/callum-laing" target="_blank">Github</a
        ></span
      >
      <span class="linkIcon"
        ><a href="https://www.linkedin.com/in/callumlaing91/" target="_blank"
          >Linkedin</a
        ></span
      >
      <!-- <span class="linkIcon"
        ><a href="https://callum-laing.github.io/resume/" target="_blank"
          >Resume</a
        ></span 
      > -->
    </div>
    <h2>©2024 Callum Laing</h2>
  </div>
</main>

<style>
  .footer {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-bottom: 15px;
    padding-top: 15px;
    backdrop-filter: blur(20px);
    background: rgba(255, 255, 255, 0.07);
  }

  h2 {
    font-size: 1rem;
    margin-left: 25px;
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  a {
    text-decoration: none;
    font-size: 1.2em;
    color: rgba(200, 255, 200);
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    margin: 10px;
  }

  a:hover {
    border-bottom: 2px solid rgba(237, 232, 187);
  }

  @media (max-width: 768px) {
    h2 {
      font-size: 0.8rem;
      margin-left: none;
    }
    .linkIcon {
      font-size: 0.8rem;
      width: 100%;
    }
    a {
      padding: 5px;
    }
  }
</style>
