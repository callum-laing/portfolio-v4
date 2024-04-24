<script>
    function scrollToElement(event) {
        event.preventDefault();
        const targetId = event.target.getAttribute('href').substring(1);
        const targetElement = document.getElementById(targetId);
        if (targetElement) {
            targetElement.scrollIntoView({
                behavior: 'smooth',
                block: 'start'
            });
        }
    }
</script>

<nav>
    <div class="links">
        <a href="#projects" on:click={scrollToElement}>Projects</a>
        <a href="#about" on:click={scrollToElement}>About</a>
        <a href="#contactContainer" on:click={scrollToElement}>Contact</a>
    </div>
</nav>

<style>
    nav {
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding-bottom: 25px;
        padding-top: 25px;
        backdrop-filter: blur(20px);
        background: rgba(255,255,255,0.07);
        border-bottom: 1px solid rgba(255,255,255,0.3);
    }

    a {
        text-decoration: none;
        margin-left: 20px;
        font-size: 1.2em;
    }

    a:hover {
        border-bottom: 2px solid yellow;
        color: rgba(200, 200, 200);
    }


	.links {
		letter-spacing: 2px;
	}

@media (max-width: 769px) {
    nav {
        display: flex;
        justify-content: space-around;
    } h1 {
        display: none;
    } a {
        font-size: 0.8em;
    }
}
</style>