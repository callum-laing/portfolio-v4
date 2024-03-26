<script>

</script>

<main>
    <div class="links">
        <a href="#projects">Projects</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a></div>

</main>

<style>
    main {
        display: flex;
        justify-content: space-around;
        align-items: center;
        color: white;
        margin-bottom: 100px;
        margin-top: 25px;
    }

    a {
        text-decoration: none;
        color: white;
        margin-left: 20px;
        font-size: 1.2em;
    }

    a:hover {
        border-bottom: 2px solid yellow;
    }


	.links {
		letter-spacing: 2px;
	}

@media (max-width: 769px) {
    main {
        display: flex;
        justify-content: space-around;
    } h1 {
        display: none;
    } a {
        font-size: 0.8em;
    }
}
</style>