<script>
    import github from '../assets/svg/github.svg';
    import linkedin from '../assets/svg/linkedin.svg';
</script>

<main>
    <div class="footer">
        <div class="links">
            <span class="linkIcon"><a href="https://github.com/callum-laing">Github</a></span>
            <span class="linkIcon"><a href="https://www.linkedin.com/in/callumlaing91/">Linkedin</a></span>
            <span class="linkIcon"><a href="https://callum-laing.github.io/resume/">Resume</a></span>
        </div>
        <h2>©2024 Callum Laing</h2>
    </div>
</main>

<style>

.footer {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 100px;
    border-top: 1px solid white;
    padding: 20px;
}

h2 {
    font-size: 1rem;
    margin-left: 25px;
}

a {
    text-decoration: none;
    padding: 10px;
}

a:hover  {
    color: yellow;
}

@media (max-width: 769px) {
    h2 {
        font-size: 0.5em;
        margin-left: none;
    }
    .linkIcon {
        font-size: 0.5em;
        width: 100%;
    }
    a {
        padding: 0;
    }
}
</style>