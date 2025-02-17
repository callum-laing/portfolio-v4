<script>
	import html from '../assets/svg/htmlsvg.svg';
	import css from '../assets/svg/csssvg.svg';
	import scss from '../assets/svg/scsssvg.svg';
	import tailwind from '../assets/svg/tailwindsvg.svg';
	import javascript from '../assets/svg/javascriptsvg.svg';
	import react from '../assets/svg/reactsvg.svg';
	import svelte from '../assets/svg/sveltesvg.svg';
	import vue from '../assets/svg/vuesvg.svg';
	import git from '../assets/svg/gitsvg.svg';
	import github from '../assets/svg/githubsvg.svg';
	import vscode from '../assets/svg/vscodesvg.svg';
	import vite from '../assets/svg/vitesvg.svg';
	import nuxt from '../assets/svg/nuxt.svg';
	import powerbi from '../assets/svg/powerbisvg.svg';
	import sql from '../assets/svg/sql.svg';
	import python from '../assets/svg/python.svg';
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
			<!-- <div class="skill-item">
        <img src={scss} alt="SCSS Icon" />
        <p>SCSS</p>
      </div> -->
			<!-- <div class="skill-item">
				<img src={tailwind} alt="Tailwind Icon" />
				<p>Tailwind</p>
			</div> -->
			<div class="skill-item">
				<img src={javascript} alt="JavaScript Icon" />
				<p>JavaScript</p>
			</div>
			<div class="skill-item">
				<img src={vue} alt="Vue Icon" />
				<p>Vue</p>
			</div>
			<!-- <div class="skill-item">
				<img src={nuxt} alt="Nuxt Icon" />
				<p>Nuxt</p>
			</div> -->
			<div class="skill-item">
				<img src={svelte} alt="Svelte Icon" />
				<p>Svelte</p>
			</div>
			<div class="skill-item">
				<img src={react} alt="React Icon" />
				<p>React</p>
			</div>
			<!-- <div class="skill-item">
				<img src={python} alt="Python Icon" />
				<p>Python</p>
			</div> -->
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
				<img src={vite} alt="Vite Icon" />
				<p>Vite</p>
			</div>
			<div class="skill-item">
				<img src={sql} alt="SQL Icon" />
				<p>SQL</p>
			</div>
			<div class="skill-item">
				<img src={powerbi} alt="PowerBI Icon" />
				<p>PowerBI</p>
			</div>
		</div>
	</div>

	<div class="about-half">
		<h2>About</h2>
		<span>
			<p>
				Hi there! I’m a front-end web developer with a passion for turning ideas into reality. My
				journey into web development started with a simple curiosity about how the web works, which
				soon grew into a love for building sleek, responsive designs that are both functional and
				visually engaging.
			</p>
			<br />
			<p>
				I enjoy the challenge of problem-solving and the satisfaction of seeing a project come
				together. Whether it’s refining a user interface or making sure a site works seamlessly
				across devices, I take pride in creating clean, efficient code and delivering experiences
				that are intuitive and accessible.
			</p>
			<br />
			<p>
				When I’m not coding, I like staying active by hitting the gym, hiking, or playing sports.
				I’m also a big fan of unwinding with a good movie or two. These interests keep me balanced
				and energized, and I find they often inspire fresh ideas in my work.
			</p>
		</span>
	</div>
</section>

<style>
	.about {
		min-height: 100dvh;
		/* background: rgb(26, 25, 25); */
		display: grid;
		grid-template-columns: 1fr 1fr;
		align-items: flex-start;
		padding: 2em;
		gap: 2em;
	}

	.skills-half,
	.about-half {
		text-align: center;
		color: rgba(199, 199, 199);
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
		box-shadow: 0 6px 8px rgba(0, 0, 0, 0.4);
		display: flex;
		align-items: center;
		gap: 10px;
		border-radius: 5px;
		padding: 5px;
		justify-content: center;
		transition: 0.3s ease;
	}

	.skill-item:hover {
		box-shadow: 1px 1px black;
		cursor: pointer;
	}

	.skill-item img {
		width: 34px;
		height: 34px;
	}

	h2 {
		font-size: 5rem;
		margin-bottom: 1em;
		font-weight: 600;
		text-decoration-line: underline;
		text-decoration-color: rgb(81, 139, 179);
		text-decoration-thickness: 5px;
		text-underline-offset: 5px;
	}

	p {
		font-size: 1.2rem;
		margin: 0.5em 0;
		max-width: 600px;
		margin-left: auto;
		margin-right: auto;
		text-align: start;
	}

	/* Responsive Styles */
	@media (max-width: 768px) {
		.about {
			grid-template-columns: 1fr;
			padding: 1em;
			gap: 5em;
			padding-top: 10em;
			padding-bottom: 10em;
			background: rgb(26, 25, 25);
		}

		h2 {
			font-size: 5rem;
			text-decoration-line: underline;
			text-decoration-color: rgb(81, 139, 179);
			text-decoration-thickness: 5px;
			text-underline-offset: 5px;
		}

		h2,
		p {
			color: rgb(200, 200, 200);
		}

		.skills-flex {
			grid-template-columns: repeat(2, 1fr);
		}

		.skill-item {
			padding: 10px;
			max-width: 90%;
		}

		.about-half {
			display: flex;
			flex-direction: column;
			line-height: 1.5;
		}

		p {
			font-size: 1rem;
			text-align: start;
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
