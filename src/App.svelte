<script>
  import "./app.css";

  // import Background from "./components/Background.svelte";
  import Navbar from "./components/Navbar.svelte";
  import Hero from "./components/Hero.svelte";
  import Projects from "./components/Projects.svelte";
  import ContactMe from "./components/ContactMe.svelte";
</script>

<main>
  <!-- <Background /> -->
  <Navbar />
  <Hero />
  <Projects />
  <ContactMe />
</main>

<style>
  main {
    margin: auto;
    width: 100%;
  }
</style>
