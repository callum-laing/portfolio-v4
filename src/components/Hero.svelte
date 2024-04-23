<script>
    import cal from '../assets/contactImages/cal.jpg';
</script>


<main>
    <div class="intro">
        <h1>Hey, I'm Callum.</h1>
        <p class="subtitle">Front-End Developer in Cambridge, UK.</p>
        <p class="heroTxt">I'm on a journey of creating responsive, dynamic and intuitive online experiences—one pixel at a time.</p>
    </div>
    <div>
        <img src={cal} alt="">
    </div>
</main>

<style>
 main {
    display: flex;
    height: 100vh;
    justify-content: center;
    align-items: center;
 }
    
    .intro {
        font-size: 3rem;
        width: 50%;
    }
    
    h1 {
        font-size: 6rem;
        margin: 0;
    }
    
    .subtitle {
        font-size: 0.5em;
        font-weight: 400;
        color: yellow;
        margin: 0;
    }
    .heroTxt {
        font-size: 0.8em;
    }
 img {
    width: auto;
    height: 400px;
 }


    @media (max-width: 769px) {
        .intro {
            height: 100%;
        }
        h1 {
            font-size: 5rem;
        } img {
            display: none;
        }
    }

    @media (min-width: 770px)and (max-width: 1024px) {
    }
</style>