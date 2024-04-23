<script>
    import cal from '../assets/contactImages/cal.jpg';
    import calFootball from '../assets/calFootball.jpg';
</script>


<div id="heroWrapper">
    <div class="intro">
        <h1>Hey,<br> I'm Callum.</h1>
        <p class="subtitle">Front-End Developer in Cambridge, UK.</p>
        <p class="heroTxt">I'm on a journey of creating responsive, dynamic and intuitive online experiences—one pixel at a time.</p>
    </div>
        <img class="calImg" src={cal} alt="">
        <!-- <img class="footballImg" src={calFootball} alt=""> -->
</div>

<style>
 #heroWrapper {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    padding-top: 150px;
    padding-bottom: 250px;
 }
    
.intro {
        font-size: 3rem;
        width: 40%;
        padding-right: 20px;
}
    
h1 {
        font-size: 8rem;
        margin: 0;
}
    
.subtitle {
        font-size: 0.5em;
        font-weight: 400;
        color: yellow;
        margin: 0;
}
.heroTxt {
        font-size: 0.6em;
}

 img {
    width: auto;
    height: 400px;
    border-radius: 10px;
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