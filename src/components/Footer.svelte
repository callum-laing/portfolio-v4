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
      <span class="linkIcon"
        ><a href="https://callum-laing.github.io/resume/" target="_blank"
          >Resume</a
        ></span
      >
    </div>
    <h2>©2024 Callum Laing</h2>
  </div>
</main>

<style>
  .footer {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-bottom: 25px;
    padding-top: 25px;
    backdrop-filter: blur(20px);
    background: rgba(255, 255, 255, 0.07);
    border-top: 1px solid rgba(255, 255, 255, 0.3);
  }

  h2 {
    font-size: 1rem;
    margin-left: 25px;
  }

  a {
    text-decoration: none;
    padding: 10px;
  }

  a:hover {
    border-bottom: 2px solid yellow;
    color: rgba(200, 200, 200);
  }

  @media (max-width: 769px) {
    h2 {
      font-size: 1em;
      margin-left: none;
    }
    .linkIcon {
      font-size: 1em;
      width: 100%;
    }
    a {
      padding: 5px;
    }
  }
</style>
