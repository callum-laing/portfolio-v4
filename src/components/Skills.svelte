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
    import git from '../assets/svg/git.svg';
    import github from '../assets/svg/github.svg';

</script>

<h1 class="skillsTitle">My Toolbox</h1>
<p>Below are the skills and tools I use to bring projects to life:</p>
<div class="skillsContainer">
    <div class="skillIcons">
        <img src={html} alt="html icon">
		<i>HTML5</i>
	</div>
	<div class="skillIcons">
        <img src={css} alt="css icon">
		<i>CSS3</i>
	</div>
	<div class="skillIcons">
        <img src={javascript} alt="javascript icon">
		<i>JavaScript</i>
	</div>
	<div class="skillIcons">
        <img src={svelte} alt="svelte icon">
		<i>Svelte</i>
	</div>
	<div class="skillIcons">
        <img src={react} alt="react icon">
        <i>React</i>
	</div>
    <div class="skillIcons">
        <img src={nextjs} alt="nextjs icon">
        <i>Next</i>
	</div>
    <div class="skillIcons">
        <img src={vite} alt="vite icon">
        <i>Vite</i>
	</div>
    <div class="skillIcons">
        <img src={git} alt="git icon">
        <i>Git</i>
	</div>
    <div class="skillIcons">
        <img src={github} alt="github icon">
        <i>Github</i>
	</div>

    <div class="skillIcons">
        <img src={cloudflare} alt="cloudflare icon">
        <i>Cloudflare</i>
	</div>
    <div class="skillIcons">
        <img src={vscode} alt="vscode icon">
        <i>VS Code</i>
	</div>
    <div class="skillIcons">
        <img src={responsive} alt="responsive icon">
        <i>Responsive Design</i>
	</div>


</div>

<style>

    .skillsTitle {
        margin-top: 100px;

    }

.skillsContainer {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        margin-bottom: 100px;
    }


.skillIcons {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 10px;
        margin-bottom: 50px;
        width: calc(100% / 10);
        margin-left: 50px;
        margin-right: 50px;
    }


img {
    width: 50px;
}
p {
    font-style: italic;
}

i {
    color: white;
    font-style: normal;
}

</style>