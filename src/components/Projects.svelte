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
      <img src={shop} alt="" />
      <p>
        Crafted an intuitive shopping cart platform for seamless online shopping
        experiences.
      </p>
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
      <img src={memoryCard} alt="" />
      <p>
        Created a memory card game to test memory skills and provide enjoyable
        entertainment.
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
    <div class="projThree projCard">
      <h2>Todo List</h2>
      <img src={todoList} alt="" />
      <p>
        Designed a straightforward to-do list app for organizing tasks and
        boosting productivity.
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
    <!-- <div class="projFour projCard">
      <h2>Tic Tac Toe</h2>
      <img src={ticTacToe} alt="" />
      <p>
        Developed a classic Tic-Tac-Toe game for nostalgic fun and strategic
        challenges.
      </p>
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
    </div> -->
  </div>
</div>

<style>
  h1 {
    font-size: 4em;
    margin: 0;
    display: inline-block;
    background-image: linear-gradient(
      to right,
      rgba(237, 232, 187),
      rgba(237, 232, 187)
    );
    background-size: 100% 2px;
    background-position: bottom;
    background-repeat: no-repeat;
    margin-bottom: 25px;
  }

  #projects {
    padding-left: 50px;
    padding-right: 50px;
    padding-top: 50px;
    padding-bottom: 50px;
  }

  .projectWrapper {
    display: grid;
    grid-template-columns: 1fr;
    justify-content: center;
    gap: 100px;
    width: 100%;
    flex-wrap: wrap;
  }

  .projCard {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    /* border-bottom: 1px solid rgba(237, 232, 187);
    backdrop-filter: blur(20px);
    background: rgba(255, 255, 255, 0.07);
    border-radius: 8px;
    border: 2px solid rgba(255, 255, 255, 0.3); */
  }

  .projCard > p {
    word-wrap: break-word;
    text-align: center;
    font-style: italic;
  }

  img {
    width: 50%;
    height: auto;
    filter: brightness(0.8);
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    border-radius: 10px;
  }

  a {
    margin: 20px;
    text-decoration: none;
    color: rgba(200, 255, 200);
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
  }

  a:hover {
    border-bottom: 2px solid rgba(237, 232, 187);
  }

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
