<script>
  import html from "../assets/svg/htmlsvg.svg";
  import css from "../assets/svg/csssvg.svg";
  import scss from "../assets/svg/scsssvg.svg";
  import tailwind from "../assets/svg/tailwindsvg.svg";
  import javascript from "../assets/svg/javascriptsvg.svg";
  import react from "../assets/svg/reactsvg.svg";
  import svelte from "../assets/svg/sveltesvg.svg";
  import vue from "../assets/svg/vuesvg.svg";
  import git from "../assets/svg/gitsvg.svg";
  import github from "../assets/svg/githubsvg.svg";
  import vscode from "../assets/svg/vscodesvg.svg";
  import cloudflare from "../assets/svg/cloudflaresvg.svg";
  import netlify from "../assets/svg/netlifysvg.svg";
  import vite from "../assets/svg/vitesvg.svg";
</script>

<section id="aboutSection" class="about">
  <div class="skills-half">
    <h2>Skills</h2>
    <div class="skills-flex">
      <div class="skill-item">
        <img src={html} alt="HTML Icon" />
        <p>HTML</p>
      </div>
      <div class="skill-item">
        <img src={css} alt="CSS Icon" />
        <p>CSS</p>
      </div>
      <div class="skill-item">
        <img src={scss} alt="SCSS Icon" />
        <p>SCSS</p>
      </div>
      <div class="skill-item">
        <img src={tailwind} alt="Tailwind Icon" />
        <p>Tailwind</p>
      </div>
      <div class="skill-item">
        <img src={javascript} alt="JavaScript Icon" />
        <p>JavaScript</p>
      </div>
      <div class="skill-item">
        <img src={react} alt="React Icon" />
        <p>React</p>
      </div>
      <div class="skill-item">
        <img src={svelte} alt="Svelte Icon" />
        <p>Svelte</p>
      </div>
      <div class="skill-item">
        <img src={vue} alt="Vue Icon" />
        <p>Vue</p>
      </div>
      <div class="skill-item">
        <img src={git} alt="Git Icon" />
        <p>Git</p>
      </div>
      <div class="skill-item">
        <img src={github} alt="GitHub Icon" />
        <p>GitHub</p>
      </div>
      <div class="skill-item">
        <img src={vscode} alt="VSCode Icon" />
        <p>VSCode</p>
      </div>
      <div class="skill-item">
        <img src={cloudflare} alt="Cloudflare Icon" />
        <p>Cloudflare</p>
      </div>
      <div class="skill-item">
        <img src={netlify} alt="Netlify Icon" />
        <p>Netlify</p>
      </div>
      <div class="skill-item">
        <img src={vite} alt="Vite Icon" />
        <p>Vite</p>
      </div>
    </div>
  </div>

  <div class="about-half">
    <h2>About Me</h2>
    <p>
      I'm a front-end developer with a background in administration and account
      management, where I honed my communication skills working with clients,
      stakeholders, and team members. Years of playing team sports have shaped
      my adaptability, resilience, and goal-oriented mindset—qualities I bring
      to each project.
    </p>
    <p>
      I’m passionate about creating user-friendly, visually appealing
      applications and thrive on the challenge of translating design into
      responsive, dynamic interfaces. Whether collaborating or working
      independently, I’m dedicated to delivering quality results on time while
      continually expanding my front-end expertise.
    </p>
  </div>
</section>

<style>
  .about {
    min-height: 100dvh;
    /* background: linear-gradient(
      to bottom,
      rgb(26, 25, 25) 0%,
      rgb(181, 125, 125) 50%,
      rgb(26, 25, 25) 100%
    ); */
    background: linear-gradient(
      to bottom,
      rgb(26, 25, 25) 0%,
      rgb(26, 25, 25) 15%,
      rgb(81, 139, 179) 50%,
      rgb(81, 139, 179) 50%,
      rgb(26, 25, 25) 85%
    );
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    padding: 2em;
    gap: 2em;
  }

  .skills-half,
  .about-half {
    text-align: center;
    color: black;
  }

  .skills-flex {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
    gap: 30px;
    margin-top: 1em;
  }

  .skill-item {
    border: 2px solid rgba(250, 250, 250, 0.1);
    background-color: rgba(100, 100, 100, 0.4);
    box-shadow: 2px 4px 4px black;
    display: flex;
    align-items: center;
    gap: 10px;
    border-radius: 5px;
    padding: 5px;
    justify-content: center;
    transition: 0.3s ease;
  }

  .skill-item:hover {
    box-shadow: none;
    border: none;
  }

  .skill-item img {
    width: 34px;
    height: 34px;
  }

  h2 {
    margin-bottom: 0.5em;
    font-size: 5rem;
  }

  p {
    font-size: 1.2rem;
    margin: 0.5em 0;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
  }

  /* Responsive Styles */
  @media (max-width: 768px) {
    .about {
      grid-template-columns: 1fr;
      padding: 1em;
      padding-top: 10em;
      padding-bottom: 10em;
      gap: 10em;
    }

    h2 {
      font-size: 3rem;
    }

    .skills-flex {
      grid-template-columns: repeat(2, 1fr);
    }

    .skill-item {
      padding: 10px;
      max-width: 90%;
    }

    p {
      font-size: 1rem;
    }
  }

  @media (min-width: 769px) and (max-width: 1024px) {
    h2 {
      font-size: 4rem;
    }

    .skills-flex {
      grid-template-columns: repeat(2, 1fr);
    }

    p {
      font-size: 1.1rem;
    }
  }

  @media (min-width: 1025px) {
    .skills-flex {
      grid-template-columns: repeat(3, 1fr);
    }
  }
</style>
