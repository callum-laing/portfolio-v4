<script>
	import html from '../assets/svg/html.svg';
	import css from '../assets/svg/css.svg';
	import javascript from '../assets/svg/javascript.svg';
	import react from '../assets/svg/react.svg';
	import svelte from '../assets/svg/svelte.svg';
	import vite from '../assets/svg/vite.svg';
	import vscode from '../assets/svg/vscode.svg';
	import cloudflare from '../assets/svg/cloudflare.svg';
	import nextjs from '../assets/svg/next.svg';
	import git from '../assets/svg/git.svg';
	import github from '../assets/svg/github.svg';
</script>

<h1 class="skillsTitle">My Toolbox</h1>
<p>Below are the skills and tools I use to bring projects to life:</p>
<div class="skillsContainer">
	<div class="skillIcons">
		<img src={html} alt="html icon" width="50" height="auto" loading="lazy" />
		<span>HTML5</span>
	</div>
	<div class="skillIcons">
		<img src={css} alt="css icon" width="50" height="auto" loading="lazy" />
		<span>CSS3</span>
	</div>
	<div class="skillIcons">
		<img src={javascript} alt="javascript icon" width="50" height="auto" loading="lazy" />
		<span>JavaScript</span>
	</div>
	<div class="skillIcons">
		<img src={svelte} alt="svelte icon" width="50" height="auto" loading="lazy" />
		<span>Svelte</span>
	</div>
	<div class="skillIcons">
		<img src={react} alt="react icon" width="50" height="auto" loading="lazy" />
		<span>React</span>
	</div>
	<!-- <div class="skillIcons">
    <img
      src={nextjs}
      alt="nextjs icon"
      width="50"
      height="auto"
      loading="lazy"
    />
    <span>Next</span>
  </div> -->
	<div class="skillIcons">
		<img src={vite} alt="vite icon" width="50" height="auto" loading="lazy" />
		<span>Vite</span>
	</div>
	<div class="skillIcons">
		<img src={git} alt="git icon" width="50" height="auto" loading="lazy" />
		<span>Git</span>
	</div>
	<div class="skillIcons">
		<img src={github} alt="github icon" width="50" height="auto" loading="lazy" />
		<span>Github</span>
	</div>

	<div class="skillIcons">
		<img src={cloudflare} alt="cloudflare icon" width="50" />
		<span>Cloudflare</span>
	</div>
	<div class="skillIcons">
		<img src={vscode} alt="vscode icon" width="50" />
		<span>VS Code</span>
	</div>
</div>

<style>
	.skillsTitle {
		margin-top: 150px;
		display: inline-block;
		background-image: linear-gradient(to right, yellow, yellow);
		background-size: 100% 2px;
		background-position: bottom;
		background-repeat: no-repeat;
		margin-bottom: 0;
	}

	.skillsContainer {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		margin-bottom: 100px;
		backdrop-filter: blur(10px);
		background: rgba(0, 0, 0, 0);
		padding-block: 50px;
	}

	.skillIcons {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 10px;
		margin-bottom: 50px;
		width: calc(100% / 10);
		margin-left: 50px;
		margin-right: 50px;
	}

	p {
		font-style: italic;
		margin-bottom: 100px;
	}

	span {
		color: white;
		font-style: normal;
	}

	@media (max-width: 769px) {
		.skillIcons {
			width: calc(100% / 12);
			margin-left: 30px;
			margin-right: 30px;
		}
		img {
			width: 20px;
		}
		span {
			font-size: 0.8em;
		}
		h1 {
			font-size: 2rem;
		}
	}
</style>
