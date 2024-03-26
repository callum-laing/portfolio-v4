<script>
  import './app.css';


import Background from './components/Background.svelte';
import Navbar from './components/Navbar.svelte';
import Hero from './components/Hero.svelte';
import Projects from './components/Projects.svelte';
import Skills from './components/Skills.svelte';
import About from './components/About.svelte';
import Contact from './components/Contact.svelte';

</script>

<main>
<Background />
<Navbar />
<Hero />
<Projects />
<Skills />
<About />
<Contact />

</main>

<style>
main {
  margin-left: 75px;
  margin-right: 75px;
}
</style>