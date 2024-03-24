<script>
    import cal from '../assets/cal.jpg';
    import callum from '../assets/callum.jpg';
    import calFootball from '../assets/calFootball.jpg';
    import { fly } from 'svelte/transition';

  let isVisible = false;

  // Set isVisible to true after a delay to trigger the transition
  setTimeout(() => {
    isVisible = true;
  }, 1000); // Adjust the delay as needed
</script>

<main>
    {#if isVisible}
    <div class="intro">
        <h1 transition:fly="{{ x: 0, y: 100, duration: 500, delay: 500}}">Hey, I'm Callum.</h1>
        <h2 transition:fly="{{ x: 0, y: 100, duration: 750, delay: 1500}}">I'm a front-end developer based in Cambridge, UK.</h2>
        <p transition:fly="{{ x: 0, y: 100, duration: 1000, delay: 2500}}">I've combined my love for sports with a passion for web development, embarking on a journey of creating responsive, dynamic and intuitive online experiences—one pixel at a time.</p>
    </div>
    <div class="gallery">
        <img transition:fly="{{ x: 0, y: 100, duration: 1000, delay: 2500}}" src={cal} alt="">
        <img transition:fly="{{ x: 0, y: 100, duration: 1000, delay: 2500}}" src={calFootball} alt="">
        <img transition:fly="{{ x: 0, y: 100, duration: 1000, delay: 2500}}" src={callum} alt="">
    </div>
    {/if}
</main>

<style>

    
    .intro {
        font-size: 2rem;
        width: 75%;
    }
    
    h1 {
        font-size: 3rem;
        margin: 0;
    }
    
    h2 {
        font-size: 0.5em;
        font-weight: 400;
        color: yellow;
        margin: 0;
    }
    p {
        font-size: 0.8em;
    }
    
    .gallery {
        display: flex;
        align-items: center;
        justify-content: space-around;
        margin-top: 100px;
    }
    
    img {
        width: 400px;
        height: 300px;
        border-radius: 10%;
        filter: brightness(0.8);
        box-shadow: 1px 2px 2px 2px;
    }


    @media (max-width: 769px) {
        .intro {
            font-size: 1rem;
            width: 100%; }
        .gallery {
                flex-direction: column;
            }
        .gallery img:not(:first-child) {
            display: none;
        }     
        h2 {
            font-size: 0.9em;
        }
        p {
            font-size: 1em;
        }
    }
</style>