<script>
    import todoList from '../assets/todoList.jpg';
    import ticTacToe from '../assets/ticTacToe.jpg';
    import rps from '../assets/rps.jpg';
    import memoryCard from '../assets/memoryCard.jpg';
    import etchASketch from '../assets/etchASketch.jpg';
    import calculator from '../assets/calculator.jpg';
</script>

<div class="projectSection">
    <!-- <h1>Projects</h1> -->
    <div class="projectWrapper">
        <div class="projOne projCard">
            <h2>Memory Card</h2>
            <img src={memoryCard} alt="">
            <p>Created a memory card game to test memory skills and provide enjoyable entertainment.</p>
            <span>
                <a href="https://sv-memory-card.pages.dev/">Live Demo</a>
                <a href="https://github.com/callum-laing/sv-memory-card">Github Repo</a>
            </span>
        </div>
        <div class="projTWo projCard">
            <h2>Todo List</h2>
            <img src={todoList} alt="">
            <p>Designed a straightforward to-do list app for organizing tasks and boosting productivity.</p>
            <span>
                <a href="https://svelte-todo-app-73m.pages.dev/">Live Demo</a>
                <a href="https://github.com/callum-laing/svelte-todo-app">Github Repo</a>
            </span>
        </div>
        <div class="projThree projCard">
            <h2>Tic Tac Toe</h2>
            <img src={ticTacToe} alt="">
            <p>Developed a classic Tic-Tac-Toe game for nostalgic fun and strategic challenges.</p>
            <span>
                <a href="https://callum-laing.github.io/tic-tac-toe/">Live Demo</a>
                <a href="https://github.com/callum-laing/tic-tac-toe">Github Repo</a>
            </span>
        </div>
        <div class="projFour projCard">
            <h2>Rock, Paper, Scissors</h2>
            <img src={rps} alt="">
            <p>Engineered a playful Rock, Paper, Scissors game for casual gaming sessions.</p>
            <span>
                <a href="https://callum-laing.github.io/rock-paper-scissors/">Live Demo</a>
                <a href="https://github.com/callum-laing/rock-paper-scissors">Github Repo</a>
            </span>
        </div>
        <div class="projFive projCard">
            <h2>Etch-A-Sketch</h2>
            <img src={etchASketch} alt="">
            <p>Crafted an interactive Etch-a-Sketch platform for doodling and creativity.</p>
            <span>
                <a href="https://callum-laing.github.io/etch-a-sketch/">Live Demo</a>
                <a href="https://github.com/callum-laing/etch-a-sketch">Github Repo</a>
            </span>
        </div>
        <div class="projSix projCard">
            <h2>Calculator</h2>
            <img src={calculator} alt="">
            <p>Built a simple yet efficient calculator application to handle everyday arithmetic tasks with ease.</p>
            <span>
                <a href="https://callum-laing.github.io/calculator/">Live Demo</a>
                <a href="https://github.com/callum-laing/calculator">Github Repo</a>
            </span>
        </div>

    </div>
</div>

<style>

    .projectSection {
        margin-top: 100px;
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
        align-items: flex-start;   
        padding: 20px; 
        border-bottom: 1px solid yellow;
    }

    .projCard > p {
        max-width: 80%;
        word-wrap: break-word;
    }

    img {
        width: 90%;
        height: 300px;
        filter: brightness(0.8);
        box-shadow: 1px 2px 2px 2px rgba(0, 0, 0, 0.1);
        border-radius: 10px;
    }

 a {
    text-decoration: none;
    margin-right: 40px;
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
    }
 }
</style>