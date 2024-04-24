<script>
    import cal from '../assets/contactImages/cal.jpg';
    import calFootball from '../assets/calFootball.jpg';
    import calfootie from '../assets/contactImages/calfootie.png';

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


<div id="heroWrapper">
    <div class="intro">
        <h1>CALLUM LAING</h1>
        <p class="subtitle">Front-End Developer in Cambridge, UK.</p>
        <button class="button-74" on:click={scrollToElement}><a href="#about"></a>About Me!</button>
    </div>
        <img class="calImg" src={calfootie} alt="">
</div>

<style>
 #heroWrapper {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    padding-top: 200px;
    padding-bottom: 250px;
 }
    
.intro {
        font-size: 3rem;
        width: 40%;
        padding-right: 20px;
        line-height: 80px;
        padding-top: 75px;
}
    
h1 {
        font-size: 8rem;
        margin: 0;
}
    
.subtitle {
        font-size: 0.5em;
        font-weight: 400;
        color: rgba(237, 232, 187);
        margin: 0;
}

 img {
    width: auto;
    height: 500px;
 }

 a {
    text-decoration: none;
    color: black;
 }

 p {
    font-family: "Roboto Condensed", sans-serif;
    font-optical-sizing: auto;
    font-style: normal;
 }
.button-74 {
  background-color: white;
  border: 2px solid #422800;
  border-radius: 10px;
  color: black;
  cursor: pointer;
  display: inline-block;
  font-weight: 600;
  font-size: 18px;
  padding: 0 18px;
  line-height: 50px;
  text-align: center;
  text-decoration: none;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.button-74:hover {
  background-color: black;
  border: none;
  box-shadow: none;
  color: white;
}

.button-74:active {
  box-shadow: #422800 2px 2px 0 0;
  transform: translate(2px, 2px);
}

@media (min-width: 768px) {
  .button-74 {
    min-width: 120px;
    padding: 0 25px;
  }
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