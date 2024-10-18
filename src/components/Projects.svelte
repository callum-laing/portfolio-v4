<script>
  import todoList from "../assets/todoList.jpg";
  import ticTacToe from "../assets/ticTacToe.jpg";
  import shop from "../assets/shop.jpg";
  import memoryCard from "../assets/memoryCard.jpg";
  import etchASketch from "../assets/etchASketch.jpg";
</script>

<div id="projects" class="projectSection">
  <h1>Projects.</h1>
  <div class="projectWrapper">
    <div class="projOne projCard">
      <h2>Shopping Cart</h2>
      <p>
        Crafted an intuitive shopping cart platform for seamless online shopping
        experiences.
      </p>
      <img src={shop} alt="" />
      <span>
        <a class="alink" href="https://shopping-site.pages.dev/" target="_blank"
          >Live Demo</a
        >
        <a
          class="alink"
          href="https://github.com/callum-laing/shopping-site"
          target="_blank">Github Repo</a
        >
      </span>
    </div>
    <div class="projTwo projCard">
      <h2>Memory Card</h2>
      <p>
        Created a memory card game to test memory skills and provide enjoyable
        entertainment.
      </p>
      <img src={memoryCard} alt="" />
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
    <div class="projThree projCard">
      <h2>Todo List</h2>
      <p>
        Designed a straightforward to-do list app for organizing tasks and
        boosting productivity.
      </p>
      <img src={todoList} alt="" />
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
    <div class="projFour projCard">
      <h2>Tic Tac Toe</h2>
      <p>
        Developed a classic Tic-Tac-Toe game for nostalgic fun and strategic
        challenges.
      </p>
      <img src={ticTacToe} alt="" />
      <span>
        <a
          class="alink"
          href="https://callum-laing.github.io/tic-tac-toe/"
          target="_blank">Live Demo</a
        >
        <a
          class="alink"
          href="https://github.com/callum-laing/tic-tac-toe"
          target="_blank">Github Repo</a
        >
      </span>
    </div>
  </div>
</div>

<style>
  h1 {
    font-size: 5em;
    margin: 0;
    text-align: center;
    text-decoration-line: underline;
    text-decoration-color: rgba(237, 232, 187);
    text-underline-offset: 0.15em;
    margin-bottom: 2em;
  }

  #projects {
    padding: 5em;
  }
  .projectWrapper {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 50px;
    width: 100%;
  }

  .projCard {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 20px;
    border-radius: 3px;
    background-color: rgba(250, 250, 250, 0.2);
  }

  .projCard > p {
    word-wrap: break-word;
    text-align: center;
    font-style: italic;
    width: 50%;
  }

  img {
    width: 30em;
    height: auto;
    filter: brightness(0.8);
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    border-radius: 3px;
  }

  a {
    margin: 20px;
    text-decoration: none;
    /* color: black;
    font-weight: bold; */
    /* color: rgba(200, 255, 200); */
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  a:hover {
    border-bottom: 2px solid rgba(237, 232, 187);
  }

  /* p {
    color: rgba(200, 200, 200);
  } */

  h2 {
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    font-style: normal;
    margin: 0 auto;
    padding-bottom: 10px;
  }

  @media (max-width: 768px) {
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
    .projectSection {
      margin-top: 50px;
      text-align: center;
    }
    h1 {
      text-align: center;
    }
  }

  @media (min-width: 769px) and (max-width: 1024px) {
    .projectWrapper {
      grid-template-columns: 1fr 1fr;
    }
    a {
      margin: 10px;
    }
    h1 {
      text-align: center;
    }
  }
</style>
