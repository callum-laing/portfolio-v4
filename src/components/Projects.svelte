<script>
	import todoList from '../assets/todoList.jpg';
	import shop from '../assets/shop.jpg';
	import memoryCard from '../assets/memoryCard.jpg';
	import cdlworkout from '../assets/cdlworkout.jpg';
</script>

<div id="projects" class="projectSection">
	<h2>Projects</h2>
	<div class="projectWrapper">
		<div class="projCard">
			<div class="card-img">
				<img src={cdlworkout} alt="CDL Workout Project" />
			</div>
			<div class="card-info">
				<h3>CDL Workout</h3>
				<p>
					Built using the Vue framework for JavaScript. I built a minimalistic workout app that I
					use on a daily basis to track my workouts.
				</p>
				<span>
					<a class="alink" href="https://cdl-workout.pages.dev/" target="_blank">Live Demo</a>
					<a class="alink" href="https://github.com/callum-laing/cdl-workout" target="_blank"
						>Github Repo</a
					>
				</span>
			</div>
		</div>

		<div class="projCard">
			<div class="card-img">
				<img src={shop} alt="Shopping Cart Project" />
			</div>
			<div class="card-info">
				<h3>Shopping Cart</h3>
				<p>
					Built a shopping cart app with React, including a homepage, shop, and cart. This project
					strengthened my React skills, especially in managing component state.
				</p>
				<span>
					<a class="alink" href="https://shopping-site.pages.dev/" target="_blank">Live Demo</a>
					<a class="alink" href="https://github.com/callum-laing/shopping-site" target="_blank"
						>Github Repo</a
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
					As a gaming enthusiast, building a game felt like a natural choice. This project was a fun
					way to put my Svelte skills to the test and create something enjoyable.
				</p>
				<span>
					<a class="alink" href="https://sv-memory-card.pages.dev/" target="_blank">Live Demo</a>
					<a class="alink" href="https://github.com/callum-laing/sv-memory-card" target="_blank"
						>Github Repo</a
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
					Life gets busy, and mentally tracking everything can be overwhelming. I built this to-do
					list app using the Svelte framework to free up my mental bandwidth for other priorities.
				</p>
				<span>
					<a class="alink" href="https://svelte-todo-app-73m.pages.dev/" target="_blank"
						>Live Demo</a
					>
					<a class="alink" href="https://github.com/callum-laing/svelte-todo-app" target="_blank"
						>Github Repo</a
					>
				</span>
			</div>
		</div>
	</div>
</div>

<style>
	#projects {
		min-height: 100vh;
		padding: 1em;
		/* background-color: rgb(26, 25, 25); */
		text-align: center;
	}

	h2 {
		font-size: 5rem;
		margin-bottom: 1em;
		font-weight: 600;
		text-decoration-line: underline;
		text-decoration-color: rgb(81, 139, 179);
		text-decoration-thickness: 5px;
		text-underline-offset: 5px;
		/* color: rgb(200, 200, 200); */
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
		font-weight: 500;
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
		border: 2px solid rgba(250, 250, 250, 0.1);
		background-color: rgba(100, 100, 100, 0.4);
		box-shadow: 0 6px 8px rgba(0, 0, 0, 0.4);
		border-radius: 5px;
		transition: 0.3s ease;
		font-weight: 600;
		margin: 0 20px;
		color: rgba(199, 199, 199);
	}

	a:hover {
		box-shadow: 1px 1px black;
		cursor: pointer;
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

	@media (max-width: 768px) {
		.alink {
			font-size: 0.8rem;
		}
	}
</style>
