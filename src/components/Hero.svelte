<script>
	import github from '../assets/svg/github2.svg';
	import linkedin from '../assets/svg/linked.svg';
	import cal from '../assets/cal.jpg';
</script>

<section class="intro-container">
	<div class="intro-left">
		<h2>Hey! I&apos;m Callum, a Web Developer based in Cambridge, UK.</h2>
		<p>
			My journey into web development started with a simple curiosity about how the web works, which
			soon grew into a love for building sleek, responsive designs that are both functional and
			visually engaging.
		</p>
		<p>
			I enjoy the challenge of problem-solving and the satisfaction of seeing a project come
			together. Whether it’s refining a user interface or making sure a site works seamlessly across
			devices, I take pride in creating clean, efficient code and delivering experiences that are
			intuitive and accessible.
		</p>
		<p>Currently seeking my next adventure as a Developer!</p>
		<div class="contactLinks">
			<a href="https://github.com/yourusername" class="githubLink" target="_blank">
				<img src={github} alt="GitHub" class="favicon" />
				View GitHub
			</a>
			<a href="https://www.linkedin.com/in/yourprofile" class="linkedinLink" target="_blank">
				<img src={linkedin} alt="LinkedIn" class="favicon" />
				View LinkedIn
			</a>
		</div>
	</div>
	<img class="cal-img" src={cal} alt="" />
</section>

<style>
	.intro-container {
		display: grid;
		grid-template-columns: 1fr 1fr;
		align-items: cente;
		width: 100%;
		max-width: 1400px;
		margin: 0 auto;
		min-height: 100svh;
		align-items: center;
	}

	/* Left text styling */
	.intro-left {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-start;
		gap: 40px;
		margin-right: -100px;
	}

	.intro-left h2 {
		font-size: 2.3em;
		font-weight: bold;
	}

	.intro-left p {
		font-size: 1.4em;
	}

	.intro-left a {
		padding: 5px 10px;
		margin-right: 20px;
		text-decoration: none;
		color: black;
		border: 1px solid rgb(120, 120, 120);
		border-radius: 5px;
		font-size: 1.2em;
		transition: 0.1s ease-in;
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
		color: rgb(200, 200, 200);
		font-weight: 600;
		transition: 0.3s ease;
		border: none;
	}

	.contactLinks > a:hover {
		color: rgb(81, 139, 179);
	}

	.cal-img {
		width: 350px;
		height: auto;
		border-radius: 10px;
		box-shadow: 1px 1px 1px 1px black;
		margin-left: 20px;
		object-fit: cover;
		justify-self: flex-end;
	}
</style>
