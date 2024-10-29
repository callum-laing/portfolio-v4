<script>
  import "./app.css";

  import Hero from "./components/Hero.svelte";
  import Projects from "./components/Projects.svelte";
  import About from "./components/About.svelte";
  import Contact from "./components/Contact.svelte";
</script>

<main>
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
</style>
