<script>
  import "./app.css";

  import Background from "./components/Background.svelte";
  import Navbar from "./components/Navbar.svelte";
  import Hero from "./components/Hero.svelte";
  import Projects from "./components/Projects.svelte";
  import Skills from "./components/Skills.svelte";
  import About from "./components/About.svelte";
  import Contact from "./components/Contact.svelte";
  import Footer from "./components/Footer.svelte";
  import Hire from "./components/Hire.svelte";
</script>

<main>
  <Background />
  <Navbar />
  <Hero />
  <Projects />
  <!-- <Hire /> -->
  <!-- <Skills /> -->
  <!-- <About /> -->
  <Contact />
  <Footer />
</main>

<style>
  main {
    margin: auto;
    width: 100%;
  }
</style>
