<script>
    import calFootball from '../assets/contactImages/calFootball.jpg';
    import fleurRock from '../assets/contactImages/fleurRock.jpg';
</script>

<div id="about"> 
    <div class="aboutWrapper">
        <div class="aboutMe">
            <h1>Who am I?</h1>
            <p>I'm a Front-End Developer with a background in sales administration and a passion for coding. By day, I'm immersed in the world of sales operations, where I thrive on ensuring seamless processes and supporting the sales team.</p>
            <p>Outside of work, I'm a sports enthusiast and enjoy playing American football at the highest level in the UK. Hiking with my partner and our dog, typically in the Scottish Highlands, is another favourite hobby of mine, allowing me to unwind and take in the breath-taking scenery.</p>
        </div>
        <div class="aboutImages">
            <img src={calFootball} alt="">
            <img src={fleurRock} alt="">
        </div>
    </div>
</div>

<style>
#about {
    padding-top: 300px;
    padding-left: 50px;
    padding-right: 50px;
}

.aboutWrapper {
    display: flex;
    align-items: center;
    gap: 40px;
}

.aboutMe {
    width: 50%;
}

.aboutImages {
    display: flex;
    gap: 40px;
    align-items: center;
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

p {
    font-size: 1.5em;
    letter-spacing: 1px;
}
img {
    width: auto;
    height: 300px;
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