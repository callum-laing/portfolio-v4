<script>
	import github from '../assets/svg/github.svg';
	import Linked from '../assets/svg/linked.svg';
</script>

<section class="contact">
	<h2>Contact</h2>
	<div id="contactContainer">
		<div class="linksSection">
			<p>
				Thanks for stopping by. I'm actively looking for work as a Web Developer. Please get in
				touch if you'd like to discuss employment opportunities.
			</p>
			<h3>My Links</h3>
			<div class="skill-item">
				<img src={github} alt="GitHub Icon" />
				<a href="https://github.com/callum-laing" target="_blank">GitHub</a>
			</div>

			<div class="skill-item">
				<img src={Linked} alt="LinkedIn Icon" />

				<a href="www.linkedin.com/in/callumlaing91" target="_blank">LinkedIn</a>
			</div>
		</div>
		<div class="formSection">
			<form action="https://formspree.io/f/xknykdjb" method="POST">
				<label for="name">
					<p class="formHeader">Your Name:</p>
					<input type="text" name="name" placeholder="What should I call you?" required />
				</label>
				<label for="email">
					<p class="formHeader">Your Email:</p>
					<input type="email" name="email" placeholder="What is your email?" required />
				</label>
				<label for="message">
					<p class="formHeader">Message:</p>
					<textarea
						rows="8"
						name="message"
						class="body"
						placeholder="Please leave your message here..."
						required
					/>
				</label>
				<button class="formSubmit" type="submit">Submit</button>
			</form>
		</div>
	</div>
</section>

<style>
	#contactContainer {
		display: flex;
		justify-content: space-between; /* Space between the two sections */
		gap: 3em;
		margin: 1em 0;
		min-height: calc(100vh - 6rem); /* Ensures the container takes full viewport height */
	}

	.formSection {
		width: 48%; /* Takes half the width */
		display: flex;
		flex-direction: column;
		gap: 1em;
		align-items: flex-start; /* Align to the top of the container */
	}

	.linksSection {
		width: 48%; /* Takes the other half of the width */
		display: flex;
		flex-direction: column;
		justify-content: flex-start; /* Aligns the content to the top */
		gap: 1em;
		align-items: flex-start; /* Aligns to the top of the container */
	}

	h2 {
		font-size: 3rem;
		font-weight: 600;
		color: white;
	}

	.formHeader {
		font-size: 1.1rem;
		padding-bottom: 5px;
		color: rgba(220, 220, 220);
		text-align: start;
	}

	form {
		display: flex;
		flex-direction: column;
		gap: 20px;
		width: 100%;
		max-width: 600px;
	}

	label {
		display: flex;
		flex-direction: column;
		font-weight: 500;
	}

	input,
	textarea {
		border: 2px solid rgba(250, 250, 250, 0.1);
		background-color: rgba(50, 50, 50, 0.4);
		box-shadow: 2px 5px 5px rgba(0, 0, 0, 0.4);
		padding: 10px;
		border-radius: 10px;
		font-size: 1em;
		color: white;
		font-family: 'Roboto', sans-serif;
	}

	input::placeholder,
	textarea::placeholder {
		color: rgba(200, 200, 200, 0.6);
	}

	textarea {
		resize: vertical;
	}

	input:focus,
	textarea:focus {
		outline: none;
		border-color: #ccc;
	}

	button.formSubmit {
		padding: 10px;
		border: none;
		border-radius: 10px;
		background-color: transparent;
		color: rgba(199, 199, 199);
		box-shadow: 2px 5px 5px rgba(0, 0, 0, 0.4);
		font-weight: 600;
		font-size: 1.2em;
		cursor: pointer;
		transition: 0.3s ease;
		width: 150px;
		border: 1px solid rgb(81, 139, 179);
	}

	button.formSubmit:hover {
		background-color: rgba(81, 139, 179, 0.8);
		box-shadow: 1px 1px rgba(0, 0, 0, 0.4);
		cursor: pointer;
	}

	.linksSection h3 {
		font-size: 1.5rem;
		color: white;
		font-weight: 600;
	}

	.linksSection ul {
		list-style: none;
		padding: 0;
	}

	.linksSection ul li {
		font-size: 1.1rem;
		color: rgba(220, 220, 220);
	}

	.linksSection ul li a {
		color: rgb(81, 139, 179);
		text-decoration: none;
	}

	.linksSection ul li a:hover {
		text-decoration: underline;
	}

	.skill-item {
		display: flex;
		align-items: center;
		transition: 0.3s ease;
		gap: 5px;
		font-weight: 600;
		line-height: 34px;
	}

	.skill-item img {
		width: 34px;
		height: 34px;
	}

	.skill-item a {
		text-decoration: none;
		color: rgba(220, 220, 220);

		margin: 0;
		line-height: 34px;
	}

	@media (max-width: 767px) {
		#contactContainer {
			flex-direction: column;
			padding: 2em 1em;
		}

		h2 {
			font-size: 2.5rem;
		}

		.formSection,
		.linksSection {
			width: 100%;
		}

		form {
			width: 80%;
		}

		input,
		textarea {
			font-size: 0.9em;
		}

		button.formSubmit {
			font-size: 1em;
		}
	}

	@media (min-width: 768px) {
		h2 {
			font-size: 4rem;
		}

		input,
		textarea {
			font-size: 1em;
		}
	}
</style>
