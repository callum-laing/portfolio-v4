<script>
	import html from '../assets/svg/htmlsvg.svg';
	import css from '../assets/svg/csssvg.svg';
	import javascript from '../assets/svg/javascriptsvg.svg';
	import react from '../assets/svg/reactsvg.svg';
	import svelte from '../assets/svg/sveltesvg.svg';
	import vue from '../assets/svg/vuesvg.svg';
	import git from '../assets/svg/gitsvg.svg';
	import vite from '../assets/svg/vitesvg.svg';
	import sql from '../assets/svg/sql.svg';
	import cloudflare from '../assets/svg/cloudflare.svg';
	import nuxt from '../assets/svg/nuxt.svg';
	import supabase from '../assets/svg/supabase.svg';
</script>

<section id="aboutSection" class="about">
	<h2>About me</h2>
	<p>
		Hi there! I’m a front-end web developer with a passion for turning ideas into reality. My
		journey into web development started with a simple curiosity about how the web works, which soon
		grew into a love for building sleek, responsive designs that are both functional and visually
		engaging.
	</p>
	<br />
	<h3>Skills & Tools:</h3>
	<div class="skill-container">
		<div class="skill-item">
			<img src={html} alt="HTML Icon" />
			<p>HTML</p>
		</div>
		<div class="skill-item">
			<img src={css} alt="CSS Icon" />
			<p>CSS</p>
		</div>
		<div class="skill-item">
			<img src={javascript} alt="JavaScript Icon" />
			<p>JavaScript</p>
		</div>
		<div class="skill-item">
			<img src={vue} alt="Vue Icon" />
			<p>Vue3</p>
		</div>
		<div class="skill-item">
			<img src={nuxt} alt="Nuxt Icon" />
			<p>Nuxt</p>
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
			<img src={sql} alt="SQL Icon" />
			<p>SQL</p>
		</div>
		<div class="skill-item">
			<img src={vite} alt="Vite Icon" />
			<p>Vite</p>
		</div>
		<div class="skill-item">
			<img src={supabase} alt="Supabase Icon" />
			<p>Supabase</p>
		</div>
		<div class="skill-item">
			<img src={cloudflare} alt="Cloudflare Icon" />
			<p>Cloudflare</p>
		</div>
		<div class="skill-item">
			<img src={git} alt="Git Icon" />
			<p>Git</p>
		</div>
	</div>
</section>

<style>
	.about {
		margin: 1em 0;
		min-height: calc(100vh - 20rem);
	}

	h2 {
		font-size: 3rem;
		margin-bottom: 0.5em;
		font-weight: 600;
		color: white;
	}

	h3 {
		font-size: 1.2em;
		font-weight: bold;
	}

	p {
		max-width: 1200px;
		line-height: 1.4;
	}

	.skill-container {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		grid-gap: 25px;
		padding: 1em 0;
	}
	.skill-item {
		display: flex;
		align-items: center;
		transition: 0.3s ease;
		gap: 5px;
		font-weight: 600;
	}

	.skill-item img {
		width: 32px;
		height: 32px;
	}

	.skill-item p {
		margin: 0;
		line-height: 25px;
	}

	/* Mobile */
	@media (max-width: 600px) {
		h2 {
			font-size: 2rem;
		}

		h3 {
			font-size: 1rem;
		}

		p {
			font-size: 0.9rem;
		}

		.skill-container {
			grid-template-columns: repeat(2, 1fr);
			grid-gap: 15px;
		}

		.skill-item img {
			width: 24px;
			height: 24px;
		}

		.skill-item p {
			font-size: 0.8rem;
		}
	}
</style>
