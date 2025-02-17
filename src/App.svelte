<script>
	import './app.css';

	import Hero from './components/Hero.svelte';
	import Projects from './components/Projects.svelte';
	import About from './components/About.svelte';
	import Contact from './components/Contact.svelte';
</script>

<main>
	<div class="nav-container">
		<h1>CALLUM LAING</h1>
		<nav>
			<a href="#projects">Projects</a>
			<a href="#aboutSection">About</a>
			<a href="#contactContainer">Contact</a>
		</nav>
	</div>
	<Hero />
	<Projects />
	<About />
	<Contact />
</main>

<style>
	main {
		margin: auto;
		width: 100%;
	}

	.nav-container {
		display: flex;
		justify-content: space-between;
		padding: 1em 15em;
		font-size: 1.2em;
	}

	nav a {
		text-decoration: none;
		padding-left: 25px;
	}
</style>
