<h1 id="contact">Get in touch</h1>
<div class="grid-wrap">
    <p class="txt">Feel free to leave me a message; I try to reply to everyone when I'm able to. Please don't spam.</p>
	<form action="https://formspree.io/f/xknykdjb" method="POST">
		<label for="subject">
			<p>Your name:</p>
			<input type="text" name="subject" placeholder="What should I call you?"/>
		</label>
        <label for="email">
			<p>Your email:</p>
			<input type="email" name="subject" placeholder="What is your email?"/>
		</label>
		<label for="body">
			<p>Message:</p>
			<textarea rows="5" name="body" class="body" placeholder="Please leave your message here..."/>
		</label>
		<button type="submit">Send</button>
	</form>
</div>

<style>
	.grid-wrap {
		display: flex;
		justify-content: center;
		align-items: center;
        flex-direction: column;
	}
	h1,
	p {
		color: white;
	}

	h1 {
		font-size: 3rem;
        margin-top: 150px;
        text-align: center;
	}

    p {
        width: 30%;
    }
	form {
		display: flex;
		flex-direction: column;
		gap: 10px;
	}

	button {
        background: transparent;
		padding: 5px;
		width: 70px;
		color: #ccd0e8;
		font-size: 1.1em;
		font-family: 'Fjalla One', sans-serif;
        border: 1px solid white;
	}

	button:hover {
		border: 1px solid yellow;
        color: yellow;
		cursor: pointer;
	}


	input,
	textarea {
		width: 600px;
        height: 30px;
		border: 2px solid white;
        padding: 2px;
		background-color: #1d2242;
		color: #ccd0e8;
		font-family: verdana;
		font-size: 0.9em;
	}

	.body {
		width: 600px;
		height: 150px;
		resize: none;
	}

	p {
		color: white;
		font-size: 1.1em;
	}

	@media (max-width: 769px) {
		.grid-wrap {
			display: flex;
			flex-direction: column;
			margin-bottom: 50px;
			gap: 20px;
		}
        input, textarea, .body {
            width: 100%;
            height: auto;
            margin: 0 auto;
        }
        h1 {
            font-size: 2rem;
        }
        p {
            width: 100%;
            padding: 0;
            margin: 0;
        }
        h1, .txt {
            text-align: center;
        }
	}

    @media (min-width: 770px) and (max-width: 1024px) {
        .txt {
            width: 50%;
            text-align: center;
        }
    }
</style>
