<script>
  import todoList from "../assets/todoList.jpg";
  import shop from "../assets/shop.jpg";
  import memoryCard from "../assets/memoryCard.jpg";
  import cdlworkout from "../assets/cdlworkout.jpg";
</script>

<div id="projects" class="projectSection">
  <h1>Projects</h1>
  <div class="projectWrapper">
    <div class="projOne projCard">
      <div class="card-info">
        <h2>Shopping Cart</h2>
        <p>
          Using the React framework, I built an intuitive shopping cart platform
          that delivers seamless online shopping experiences.
        </p>
        <span>
          <a
            class="alink"
            href="https://shopping-site.pages.dev/"
            target="_blank">Live Demo</a
          >
          <a
            class="alink"
            href="https://github.com/callum-laing/shopping-site"
            target="_blank">Github Repo</a
          >
        </span>
      </div>
      <div class="card-img">
        <img src={shop} alt="" />
      </div>
    </div>

    <div class="projTwo projCard">
      <div class="card-info">
        <h2>Memory Card</h2>
        <p>
          Created a memory card game with the React framework to test memory
          skills and provide enjoyable entertainment.
        </p>
        <span>
          <a
            class="alink"
            href="https://sv-memory-card.pages.dev/"
            target="_blank">Live Demo</a
          >
          <a
            class="alink"
            href="https://github.com/callum-laing/sv-memory-card"
            target="_blank">Github Repo</a
          >
        </span>
      </div>
      <div class="card-img">
        <img src={memoryCard} alt="" />
      </div>
    </div>

    <div class="projThree projCard">
      <div class="card-info">
        <h2>Todo List</h2>
        <p>
          Using the Svelte framework, I developed a straightforward to-do list
          project for organizing tasks and boosting productivity.
        </p>
        <span>
          <a
            class="alink"
            href="https://svelte-todo-app-73m.pages.dev/"
            target="_blank">Live Demo</a
          >
          <a
            class="alink"
            href="https://github.com/callum-laing/svelte-todo-app"
            target="_blank">Github Repo</a
          >
        </span>
      </div>
      <div class="card-img">
        <img src={todoList} alt="" />
      </div>
    </div>

    <div class="projFour projCard">
      <div class="card-info">
        <h2>CDL Workout</h2>
        <p>
          Developed a minimalistic workout project using the Vue framework to
          allow users to build customizable workout plans.
        </p>
        <span>
          <a class="alink" href="https://cdl-workout.pages.dev/" target="_blank"
            >Live Demo</a
          >
          <a
            class="alink"
            href="https://github.com/callum-laing/cdl-workout"
            target="_blank">Github Repo</a
          >
        </span>
      </div>
      <div class="card-img">
        <img src={cdlworkout} alt="" />
      </div>
    </div>
  </div>
</div>

<style>
  h1 {
    font-size: 5em;
    margin: 0;
    text-align: center;
    text-decoration-line: underline;
    text-decoration-color: black;
    text-underline-offset: 0.05em;
    text-decoration-thickness: 5px;
    margin-bottom: 2em;
    font-family: "Cormorant Garamond", serif;
    font-weight: bold;
    font-style: normal;
  }

  #projects {
    padding: 5em;
  }
  .projectWrapper {
    display: grid;
    grid-template-columns: 1fr;
    gap: 60px;
    width: 50%;
    margin: 0 auto;
  }

  .projCard {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 20px;
    border-radius: 3px;
    background-color: rgba(250, 250, 250, 0.1);
    box-shadow: 1px 1px 4px rgba(50, 50, 50);
    gap: 10px;
  }

  .card-info {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  img {
    width: 100%;
    height: auto;
    filter: brightness(0.8);
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    border-radius: 3px;
  }

  span {
    margin-bottom: 10px;
  }
  a {
    /* color: rgba(237, 232, 187); */
    padding: 20px;
    text-decoration: none;
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  a:hover {
    text-decoration-line: underline;
    text-decoration-color: rgba(50, 250, 250, 0.7);
    text-underline-offset: 0.15em;
    text-decoration-thickness: 0.2em;
  }

  h2 {
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    font-style: normal;
    margin: 0 auto;
    padding-bottom: 10px;
  }

  @media (max-width: 768px) {
    #projects {
      padding-left: 50px;
      padding-right: 50px;
      text-align: center;
    }
    .projectWrapper {
      grid-template-columns: 1fr;
    }

    img {
      width: 100%;
      height: auto;
    }
    a {
      margin: 5px;
    }

    p {
      display: none;
    }

    h1 {
      text-align: start;
      font-size: 4em;
    }
  }

  @media (min-width: 769px) and (max-width: 1024px) {
    .projectWrapper {
      grid-template-columns: 1fr;
    }
    a {
      margin: 10px;
    }
    h1 {
      text-align: center;
    }
  }
</style>
