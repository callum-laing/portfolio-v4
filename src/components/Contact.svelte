<script>
	import github from '../assets/svg/github2.svg';
	import email from '../assets/svg/email2.svg';
	import linkedin from '../assets/svg/linked.svg';
</script>

<section class="contact">
	<div id="contactContainer">
		<h2>Contact</h2>

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
				></textarea>
			</label>
			<button class="formSubmit" type="submit">Submit</button>
		</form>
	</div>
</section>

<style>
	#contactContainer {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		min-height: 100vh;
		/* background: rgb(26, 25, 25); */
		padding: 2em 1em;
		text-align: center;
	}

	h2 {
		font-size: 5rem;
		margin-bottom: 50px;
		font-weight: 600;
		text-decoration-line: underline;
		text-decoration-color: rgb(81, 139, 179);
		text-decoration-thickness: 5px;
		text-underline-offset: 5px;
	}

	.contactLinks {
		display: flex;
		gap: 50px;
		margin-bottom: 50px;
	}
	.contactLinks > a {
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 5px;
		text-decoration: none;
		font-weight: 600;
		transition: 0.3s ease;
	}

	.formHeader {
		padding-bottom: 5px;
	}

	form {
		display: flex;
		flex-direction: column;
		gap: 15px;
		width: 90%;
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
		background-color: rgba(100, 100, 100, 0.4);
		box-shadow: 2px 5px 5px black;
		padding: 10px;
		border-radius: 3px;
		font-size: 1em;
		font-family: 'Roboto', sans-serif;
	}

	input::placeholder,
	textarea::placeholder {
		opacity: 1;
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
		border-radius: 3px;
		background-color: rgb(81, 139, 179);
		border: 2px solid rgba(250, 250, 250, 0.1);
		box-shadow: 2px 5px 5px black;
		font-weight: 600;
		font-size: 1.2em;
		cursor: pointer;
		transition: 0.3s ease;
	}

	button.formSubmit:hover {
		background-color: rgba(255, 255, 255, 0.2);
		box-shadow: 1px 1px black;
		cursor: pointer;
	}
	p {
		text-align: start;
	}

	img {
		width: 25px;
	}
	@media (min-width: 768px) {
		h2 {
			font-size: 4.5rem;
		}

		form {
			width: 80%;
		}

		input {
			height: 40px;
			margin-top: 5px;
		}

		p {
			text-align: start;
		}
	}
</style>
