<div id="contactContainer">
	<h1 class="contact">Get in touch</h1>
	<p class="txt">Feel free to leave me a message; I try to reply to everyone when I'm able to. Please don't spam.</p>
	<div class="grid-wrap">
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

</div>

<style>
	#contactContainer {
	padding-left: 50px;
    padding-right: 50px;
	padding-top: 150px;
	padding-bottom: 100px;
	}

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
		display: inline-block;
		background-image: linear-gradient(to right, yellow, yellow);
    	background-size: 100% 2px;
    	background-position: bottom;
    	background-repeat: no-repeat;
		font-size: 3rem;
        margin-top: 150px;
	}

	::placeholder {
		color: rgba(209, 203, 119, 0.8);
	}
	h1 {
		margin-bottom: 0;
	}

    p {
		color: white;
		font-size: 1.1em;
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
		border: 2px solid rgba(255,255,255,0.5);
        padding: 5px;
		background-color: #1d2242;
		color: #ccd0e8;
		font-family: verdana;
		font-size: 0.9em;
		border-radius: 10px;
	}

	.body {
		width: 600px;
		height: 150px;
		resize: none;
	}


	@media (max-width: 769px) {
		.grid-wrap {
			display: flex;
			flex-direction: column;
			margin-bottom: 50px;
			gap: 10px;
		}
        input, textarea, .body {
            width: 275px;
            height: auto;
            margin: 0 auto;
        }
        h1 {
            font-size: 2rem;
        }
        p {
            width: 100%;
            margin: 0;
 		} .txt {
			padding-bottom: 10px;
			font-size: 1em;
		}
	}

    @media (min-width: 770px) and (max-width: 1024px) {
		 input, textarea {
			width: 600px;
		} p {
			width: 100%;
		}
    }
</style>
