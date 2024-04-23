<script>
    import calFootball from '../assets/contactImages/calFootball.jpg';
    import calRock from '../assets/contactImages/calRock.jpg';
    import fleurRock from '../assets/contactImages/fleurRock.jpg';
</script>

<main id="about"> 
    <div class="aboutWrapper">
        <div class="aboutMe">
            <h1>Who Am I?</h1>
            <p>I'm a Front-End Developer with a background in sales administration and a passion for coding. By day, I'm immersed in the world of sales operations, where I thrive on ensuring seamless processes and supporting the sales team.</p>
            <p>Outside of work, I'm a sports enthusiast and enjoy playing American football at the highest level in the UK. Hiking with my partner and our dog, typically in the Scottish Highlands, is another favourite hobby of mine, allowing me to unwind and take in the breath-taking scenery.</p>
            <!-- <p>When I'm not trying to sack the Quarterback in American Football, or carrying the dog up a mile high mountain in Scotland, you'll find me at the computer, expanding my skills in web development. Whether it's learning new technologies or refining my coding techniques, I'm always eager to grow and improve.</p> -->
            <!-- <p>This journey has been interesting to say the least, full of the highest highs when completing a project, to the lowest lows when spending hours looking for that bug, that usually turns out to be a missing semi-colon (thanks, JavaScript).</p> -->
        </div>
        <div class="aboutImages">
            <img src={calFootball} alt="">
            <img src={fleurRock} alt="">
            <img src={calRock} alt="">
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
        justify-content: space-between;
}

.aboutMe {
        width: 45%;
}
.aboutImages {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
}

h1 {
    font-size: 3em;
    margin: 0;
		display: inline-block;
		background-image: linear-gradient(to right, yellow, yellow);
    	background-size: 100% 2px;
    	background-position: bottom;
    	background-repeat: no-repeat;
}

img {
        width: auto;
        height: 250px;
        box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
        border-radius: 10px;
}

@media (max-width: 769px) {
    .aboutMe {
        width: 100%;
        font-size: 0.9em;
        margin-right: 0;
    }
    img {
        width: auto;
        height: 150px;
    }
    .aboutImages {
        justify-content: center;
    } h1 {
        margin-bottom: 20px;
    }
}

@media (min-width: 770px) and (max-width: 1024px) {
    .aboutMe {
        width: 100%;
    }
    img {
        width: auto;
        height: 150px;
    }
    .aboutImages {
        width: 100%;
        justify-content: center;
    }
}
</style>