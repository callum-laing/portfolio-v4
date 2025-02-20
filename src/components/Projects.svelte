<script>
	import cdlworkout from '../assets/cdlworkout.jpg';
	import todoList from '../assets/todoList.jpg';
</script>

<div id="projects" class="project-section">
	<h2>Projects</h2>
	<div class="proj-card">
		<div class="card-img">
			<img src={cdlworkout} alt="CDL Workout Project" />
		</div>
		<div class="card-info">
			<h3>CDL Workout</h3>
			<p class="card-description">
				I built a workout app using Vue.js that allows users to create workout days, add exercises
				to each day, and specify reps for each exercise. It leverages Vue's reactive state
				management to handle dynamic data updates and uses localStorage to retain workout
				information.
			</p>
			<div class="proj-card-footer">
				<p>Built using the Vue.js Framework</p>
				<div class="proj-links">
					<a class="alink" href="https://cdl-workout.pages.dev/" target="_blank">Live Demo</a>
					<a class="alink" href="https://github.com/callum-laing/cdl-workout" target="_blank"
						>Github Repo</a
					>
				</div>
			</div>
		</div>
	</div>
	<div class="proj-card">
		<div class="card-img">
			<img src={todoList} alt="Todo List" />
		</div>
		<div class="card-info">
			<h3>Todo List</h3>
			<p class="card-description">
				I built a to-do list app using Svelte.js that lets users add, edit, delete, and mark tasks
				as complete. It uses Svelte’s state management for smooth updates and stores tasks in
				localStorage so they stay saved even after closing the app.
			</p>
			<div class="proj-card-footer">
				<p>Built using the Svelte.js Framework</p>
				<div class="proj-links">
					<a class="alink" href="https://svelte-todo-app-73m.pages.dev/" target="_blank"
						>Live Demo</a
					>
					<a class="alink" href="https://github.com/callum-laing/svelte-todo-app" target="_blank"
						>Github Repo</a
					>
				</div>
			</div>
		</div>
	</div>
</div>

<style>
	#projects {
		display: flex;
		flex-direction: column;
		gap: 3em;
		margin: 1em 0;
		min-height: calc(100vh - 6rem);
	}

	h2 {
		font-size: 3rem;
	}

	h2,
	h3 {
		color: white;
		font-weight: 600;
	}

	h3 {
		margin: 0 auto;
		padding-top: 10px;
		font-size: 1.5em;
	}

	.proj-card {
		display: grid;
		grid-template-columns: 0.8fr 1fr;
		grid-gap: 25px;
		background-color: rgba(20, 20, 20);
		border-radius: 10px;
	}

	img {
		border-radius: 10px;
		box-shadow: 0 6px 8px rgba(0, 0, 0, 0.4);
		opacity: 75%;
	}
	.card-info {
		display: grid;
		grid-template-rows: 50px 1fr 50px;
	}

	.card-info p {
		line-height: 1.4;
		max-width: calc(100% - 2em);
	}

	.proj-card-footer {
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 1em;
	}

	.proj-card-footer p {
		margin: 0 auto;
		font-style: italic;
	}

	.proj-links a {
		text-decoration: none;
		color: rgba(199, 199, 199);
		transition: 0.2s ease;
		font-size: 1.1em;
		padding: 5px 10px;
		border: 1px solid rgb(81, 139, 179);
		border-radius: 10px;
	}

	.proj-links a:hover {
		color: rgb(81, 139, 179);
		border: 1px solid rgb(81, 139, 179);
	}

	@media (max-width: 767px) {
		.proj-card {
			display: flex;
			flex-direction: column;
			gap: 15px;
			padding: 1em;
		}

		.card-img {
			display: flex;
			justify-content: center;
		}

		.card-img img {
			width: 100%;
			height: auto;
			max-width: 400px;
		}

		.card-info {
			text-align: center;
			display: flex;
			flex-direction: column;
			gap: 10px;
		}

		.card-description {
			margin: 0 auto;
		}

		.proj-card-footer {
			flex-direction: column;
			gap: 10px;
		}
	}

	@media (min-width: 375px) and (max-width: 413px) {
		.proj-card {
			padding: 0.8em;
		}

		.card-info h3 {
			font-size: 1.3em;
		}

		.proj-links a {
			font-size: 0.8em;
			padding: 4px 8px;
		}
	}

	@media (max-width: 1024px) {
		.proj-card {
			display: flex;
			flex-direction: column;
			gap: 15px;
			padding: 1em;
		}

		.card-img {
			display: flex;
			justify-content: center;
		}

		.card-img img {
			width: 100%;
			height: auto;
			max-width: 500px;
		}

		.card-info {
			text-align: center;
			display: flex;
			flex-direction: column;
			gap: 10px;
		}

		.card-description {
			display: none;
		}

		.proj-card-footer {
			flex-direction: column;
			gap: 10px;
			align-items: center;
		}

		.proj-links {
			display: flex;
			gap: 10px;
			justify-content: center;
		}

		.proj-links a {
			font-size: 1em;
			padding: 5px 10px;
		}
	}
</style>
