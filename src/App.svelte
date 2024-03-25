<script>
  import './app.css';


import Background from './components/Background.svelte';
import Navbar from './components/Navbar.svelte';
import Hero from './components/Hero.svelte';
import Projects from './components/Projects.svelte';
import Skills from './components/Skills.svelte';

</script>

<main>
<Background />
<Navbar />
<Hero />
<Projects />
<Skills />

</main>

<style>
main {
  margin-left: 75px;
  margin-right: 75px;
}
</style>