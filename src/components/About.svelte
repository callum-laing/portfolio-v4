<script>
    import calFootball from '../assets/contactImages/calFootball.jpg';
    import calRock from '../assets/contactImages/calRock.jpg';
    import calWater from '../assets/contactImages/calWater.jpg';
    import fleurHike from '../assets/contactImages/fleurHike.jpg';
    import fleurRock from '../assets/contactImages/fleurRock.jpg';
    import fleurWater from '../assets/contactImages/fleurWater.jpg';
</script>

<main> 
    <div class="aboutWrapper">
        <div class="aboutMe">
            <h1 id="about">Who Am I?</h1>
            <p>I'm a Front-End Developer with a background in sales administration and a passion for coding. By day, I'm immersed in the world of sales operations, where I thrive on ensuring seamless processes and supporting the sales team.</p>
            <p>Outside of work, I'm a sports enthusiast and enjoy playing American football at the highest level in the UK. Hiking with my partner and our dog, typically in the Scottish Highlands, is another favourite hobby of mine, allowing me to unwind and take in the breath-taking scenery.</p>
            <p>When I'm not trying to sack the Quarterback in American Football, or carrying the dog up a mile high mountain in Scotland, you'll find me at the computer, expanding my skills in web development. Whether it's learning new technologies or refining my coding techniques, I'm always eager to grow and improve.</p>
            <p>This journey has been interesting to say the least, full of the highest highs when completing a project, to the lowest lows when spending hours looking for that bug, that usually turns out to be a missing semi-colon (thanks, JavaScript).</p>
        </div>
        <div class="aboutImages">
            <img src={calFootball} alt="">
            <img src={fleurWater} alt="">
            <img src={fleurHike} alt="">
            <img src={fleurRock} alt="">
            <img src={calRock} alt="">
            <img src={calWater} alt="">
        </div>
    </div>
</main>

<style>
main {
    margin-top: 150px;
}

.aboutWrapper {
        display: flex;
        flex-wrap: wrap;
}

.aboutMe {
        width: 45%;
        margin-right: 50px;
}
.aboutImages {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        gap: 10px;
        width: calc(100% / 2);
}

h1 {
    font-size: 3em;
    margin: 0;
}

img {
        width: 250px;
        height: auto;
        border-radius: 10px;
}

@media (max-width: 769px) {
    .aboutMe {
        width: 100%;
        font-size: 0.9em;
        margin-right: 0;
    }
    img {
        width: 100px;
        height: auto;
    }
    .aboutImages {
        width: 100%;
    }
}

@media (min-width: 770px) and (max-width: 1024px) {
    .aboutMe {
        width: 100%;
    }
    img {
        width: 200px;
        height: auto;
    }
    .aboutImages {
        width: 100%;
    }
}
</style>