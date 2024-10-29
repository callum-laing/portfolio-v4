<script>
  import todoList from "../assets/todoList.jpg";
  import shop from "../assets/shop.jpg";
  import memoryCard from "../assets/memoryCard.jpg";
  import cdlworkout from "../assets/cdlworkout.jpg";
</script>

<div id="projects" class="projectSection">
  <h2>Projects</h2>
  <div class="projectWrapper">
    <div class="projCard">
      <div class="card-img">
        <img src={shop} alt="Shopping Cart Project" />
      </div>
      <div class="card-info">
        <h3>Shopping Cart</h3>
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
    </div>

    <div class="projCard">
      <div class="card-img">
        <img src={memoryCard} alt="Memory Card Game" />
      </div>
      <div class="card-info">
        <h3>Memory Card</h3>
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
    </div>

    <div class="projCard">
      <div class="card-img">
        <img src={todoList} alt="To-Do List Project" />
      </div>
      <div class="card-info">
        <h3>Todo List</h3>
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
    </div>

    <div class="projCard">
      <div class="card-img">
        <img src={cdlworkout} alt="CDL Workout Project" />
      </div>
      <div class="card-info">
        <h3>CDL Workout</h3>
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
    </div>
  </div>
</div>

<style>
  body {
    margin: 0;
    padding: 0;
    font-family: "Roboto", sans-serif;
  }

  #projects {
    min-height: 100vh;
    padding: 1em;
    background-color: rgb(26, 25, 25);
    text-align: center;
  }

  h2 {
    font-size: 5rem;
    line-height: 2;
    margin-bottom: 1em;
  }

  .projectWrapper {
    display: flex;
    flex-direction: column;
    gap: 100px;
    width: 90%;
    margin: 0 auto;
  }

  .projCard {
    display: flex;
    flex-direction: column;
    padding: 15px;
    border-radius: 3px;
    background-color: rgba(250, 250, 250, 0.1);
    box-shadow: 1px 1px 4px rgba(50, 50, 50);
  }

  .card-img {
    overflow: hidden;
    position: relative;
    height: 200px;
  }

  .card-info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 10px;
  }

  h3 {
    font-size: 1.5rem;
    margin: 0.5em 0;
  }

  p {
    font-size: 1rem;
    margin: 0.5em 0;
  }

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: brightness(0.8);
    border-radius: 3px;
  }

  span {
    margin-top: 1em;
    display: flex;
    justify-content: center;
    gap: 10px;
  }

  a {
    padding: 10px 15px;
    text-decoration: none;
    color: black;
    background: rgba(255, 255, 255, 0.2);
    border-radius: 3px;
  }

  a:hover {
    text-decoration: underline;
    text-decoration-color: white;
  }

  @media (min-width: 768px) {
    .projectWrapper {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 50px;
      width: 80%;
    }

    .projCard {
      flex-direction: row;
      padding: 20px;
    }

    .card-img {
      width: 40%;
      height: auto;
      margin-right: 15px;
    }

    .card-info {
      width: 60%;
    }

    h2 {
      font-size: 5em;
    }
  }
</style>
