<script>
    import html from '../assets/svg/html.svg';
    import css from '../assets/svg/css.svg';
    import javascript from '../assets/svg/javascript.svg';
    import react from '../assets/svg/react.svg';
    import svelte from '../assets/svg/svelte.svg';

</script>

<div class="skillsContainer">
    <div class="html">
        <img src={html} alt="html icon">
		<i>HTML5</i>
	</div>
	<div class="css">
        <img src={css} alt="css icon">
		<i>CSS3</i>
	</div>
	<div class="js">
        <img src={javascript} alt="javascript icon">
		<i>JavaScript</i>
	</div>
	<div class="svelte">
        <img src={svelte} alt="svelte icon">
		<i>Svelte & Sveltekit</i>
	</div>
	<div class="react">
        <img src={react} alt="react icon">
        <i>React</i>
	</div>
</div>

<style>
    .skillsContainer {
        display: flex;
        margin-top: 100px;
        margin-bottom: 100px;
        gap: 75px;
    }

    .html, .css, .js, .react, .svelte {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 10px;
    }

    .react, .svelte {
        word-wrap: break-word;
    }
img {
    width: 50px;
}

i {
    color: white;
}

</style>