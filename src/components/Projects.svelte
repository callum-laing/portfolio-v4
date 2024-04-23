<script>
    import todoList from '../assets/todoList.jpg';
    import ticTacToe from '../assets/ticTacToe.jpg';
    import shop from '../assets/shop.jpg';
    import memoryCard from '../assets/memoryCard.jpg';
    import etchASketch from '../assets/etchASketch.jpg';
    import calculator from '../assets/calculator.jpg';
</script>

<div id="projects" class="projectSection">
    <!-- <h1>Projects</h1> -->
    <div class="projectWrapper">
        <div class="projOne projCard">
            <h2>Shopping Cart</h2>
            <img src={shop} alt="">
            <p>Crafted an intuitive shopping cart platform for seamless online shopping experiences.</p>
            <span>
                <a href="https://shopping-site.pages.dev/" target="_blank">Live Demo</a>
                <a href="https://github.com/callum-laing/shopping-site" target="_blank">Github Repo</a>
            </span>
        </div>
        <div class="projTwo projCard">
            <h2>Memory Card</h2>
            <img src={memoryCard} alt="">
            <p>Created a memory card game to test memory skills and provide enjoyable entertainment.</p>
            <span>
                <a href="https://sv-memory-card.pages.dev/" target="_blank">Live Demo</a>
                <a href="https://github.com/callum-laing/sv-memory-card" target="_blank">Github Repo</a>
            </span>
        </div>
        <div class="projThree projCard">
            <h2>Todo List</h2>
            <img src={todoList} alt="">
            <p>Designed a straightforward to-do list app for organizing tasks and boosting productivity.</p>
            <span>
                <a href="https://svelte-todo-app-73m.pages.dev/" target="_blank">Live Demo</a>
                <a href="https://github.com/callum-laing/svelte-todo-app" target="_blank">Github Repo</a>
            </span>
        </div>
        <div class="projFour projCard">
            <h2>Tic Tac Toe</h2>
            <img src={ticTacToe} alt="">
            <p>Developed a classic Tic-Tac-Toe game for nostalgic fun and strategic challenges.</p>
            <span>
                <a href="https://callum-laing.github.io/tic-tac-toe/" target="_blank">Live Demo</a>
                <a href="https://github.com/callum-laing/tic-tac-toe" target="_blank">Github Repo</a>
            </span>
        </div>

        <div class="projFive projCard">
            <h2>Etch-A-Sketch</h2>
            <img src={etchASketch} alt="">
            <p>Crafted an interactive Etch-a-Sketch platform for doodling and creativity.</p>
            <span>
                <a href="https://callum-laing.github.io/etch-a-sketch/" target="_blank">Live Demo</a>
                <a href="https://github.com/callum-laing/etch-a-sketch" target="_blank">Github Repo</a>
            </span>
        </div>
        <!-- <div class="projSix projCard">
            <h2>Calculator</h2>
            <img src={calculator} alt="">
            <p>Built a simple yet efficient calculator application to handle everyday arithmetic tasks with ease.</p>
            <span>
                <a href="https://callum-laing.github.io/calculator/" target="_blank">Live Demo</a>
                <a href="https://github.com/callum-laing/calculator" target="_blank">Github Repo</a>
            </span>
        </div> -->

    </div>
</div>

<style>

    .projectSection {
        margin-top: 150px;
    }

    .projectWrapper {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
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
        border-bottom: 1px solid yellow;
        backdrop-filter: blur(20px);
        background: rgba(255,255,255,0.07);
        border-radius: 8px;
        border: 1px solid rgba(255,255,255,0.3);
    }

    .projCard > p {
        word-wrap: break-word;
        text-align: center;
        font-style:italic;
    }

    img {
        width: 100%;
        height: auto;;
        filter: brightness(0.8);
        box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    }

 a {
    margin: 20px;
    text-decoration: none;
 }

 a:hover {
    border-bottom: 2px solid yellow;
    color: rgba(200, 200, 200);
 }

 @media (max-width: 769px) {
    .projectWrapper {
        grid-template-columns: 1fr;
    }
    img {
        width: 100%;
        height: auto;
    } a {
        margin: 5px;
    }
    .projectSection {
        margin-top: 50px;
    }
 }

 @media (min-width: 770px) and (max-width: 1024px) {
    .projectWrapper {
        grid-template-columns: 1fr 1fr;
    } a {
        margin: 10px;
    }
 }
</style>