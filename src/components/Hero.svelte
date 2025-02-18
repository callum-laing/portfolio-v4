<script>
	import cal from '../assets/calscotland.jpg';
</script>

<section class="hero">
	<img class="cal-img" src={cal} alt="" />
	<h2>Web Developer based in Cambridge, UK.</h2>
</section>

<style>
	.hero {
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		min-height: calc(100vh - 6rem);
	}

	.cal-img {
		width: 500px;
		height: auto;
		border-radius: 10px;
		object-fit: cover;
		justify-self: center;
		box-shadow: 0 6px 8px rgba(0, 0, 0, 0.4);
		opacity: 75%;
	}

	h2 {
		padding-top: 15px;
		font-size: 1.5rem;
		color: rgba(220, 220, 220);
	}

	@media (max-width: 767px) {
		h2 {
			font-size: 1rem;
		}
	}
</style>
