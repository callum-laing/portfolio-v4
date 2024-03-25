<script>
    import html from '../assets/svg/html.svg';
    import css from '../assets/svg/css.svg';
    import javascript from '../assets/svg/javascript.svg';
    import react from '../assets/svg/react.svg';
    import svelte from '../assets/svg/svelte.svg';
    import vite from '../assets/svg/vite.svg';
    import responsive from '../assets/svg/responsive.svg';
    import vscode from '../assets/svg/vscode.svg';
    import cloudflare from '../assets/svg/cloudflare.svg';
    import nextjs from '../assets/svg/next.svg';

</script>

<div class="skillsContainer">
    <h1>Skills & Tools</h1>
    <div class="html skillIcons">
        <img src={html} alt="html icon">
		<i>HTML5</i>
	</div>
	<div class="css skillIcons">
        <img src={css} alt="css icon">
		<i>CSS3</i>
	</div>
	<div class="js skillIcons">
        <img src={javascript} alt="javascript icon">
		<i>JavaScript</i>
	</div>
	<div class="svelte skillIcons">
        <img src={svelte} alt="svelte icon">
		<i>Svelte</i>
	</div>
	<div class="react skillIcons">
        <img src={react} alt="react icon">
        <i>React</i>
	</div>
    <div class="nextjs skillIcons">
        <img src={nextjs} alt="nextjs icon">
        <i>Next</i>
	</div>
    	<div class="vite skillIcons">
        <img src={vite} alt="vite icon">
        <i>Vite</i>
	</div>
    <div class="cloudflare skillIcons">
        <img src={cloudflare} alt="cloudflare icon">
        <i>Cloudflare</i>
	</div>
    <div class="vscode skillIcons">
        <img src={vscode} alt="vscode icon">
        <i>VS Code</i>
	</div>
    <div class="responsive skillIcons">
        <img src={responsive} alt="responsive icon">
        <i>Responsive Design</i>
	</div>

</div>

<style>
.skillsContainer {
        display: flex;
        margin-top: 100px;
        margin-bottom: 100px;
        gap: 75px;
    }

.skillIcons {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 10px;
    }


img {
    width: 50px;
}

i {
    color: white;
    font-style: normal;

}

</style>