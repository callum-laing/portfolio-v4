<script>
	import './app.css';

	import Hero from './components/Hero.svelte';
	import Projects from './components/Projects.svelte';
	import About from './components/About.svelte';
	import Contact from './components/Contact.svelte';
</script>

<div class="nav-container">
	<p>Callum Laing</p>
	<nav>
		<a href="#projects">Projects</a>
		<a href="#aboutSection">About</a>
		<a href="#contactContainer">Contact</a>
	</nav>
</div>

<main>
	<Hero />
	<hr />
	<About />
	<hr />
	<Projects />
	<hr />
	<Contact />
</main>

<style>
	hr {
		border-color: #f8fafc24;
	}

	main {
		margin: 0 auto;
		width: 75%;
	}

	.nav-container {
		position: sticky;
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 1em 15em;
		font-size: 1.2em;
		background: rgba(21, 21, 21);
		box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
	}

	.nav-container p {
		font-size: 1.4em;
		font-weight: bold;
		letter-spacing: 1px;
		color: rgba(220, 220, 220);
	}

	nav a {
		text-decoration: none;
		color: rgba(199, 199, 199);
		transition: 0.2s ease;
		font-size: 1.1em;
		padding: 0 10px;
	}

	nav a:hover {
		color: rgb(81, 139, 179);
	}

	@media (max-width: 767px) {
		.nav-container {
			padding: 10px 5px;
		}
		nav a {
			font-size: 0.8em;
		}
		.nav-container p {
			font-size: 1em;
		}
	}

	@media (min-width: 768px) and (max-width: 1024px) {
		.nav-container {
			padding: 15px 5px;
		}
	}

	@media (min-width: 376px) and (max-width: 430px) {
		.nav-container {
			padding: 10px 10px;
			font-size: 1em;
		}
		.nav-container p {
			font-size: 1.1em;
		}
		nav a {
			font-size: 0.9em;
		}
	}
</style>
