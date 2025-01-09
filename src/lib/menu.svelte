<script>
    import mail from '../lib/images/mail.svg';
    import github from '../lib/images/github.svg';
    import linkedin from '../lib/images/linkedin.svg';
    import sun from '../lib/images/sun.svg';
    import moon from '../lib/images/moon.svg';
    import cv from '../lib/images/cv.svg';
    import CV_ENG from '../lib/files/CV_PAUL_GUERRE_ENG.pdf';
    import { writable } from 'svelte/store';
    import { onMount } from 'svelte';

    const isLightMode = writable(false);

    const toggleTheme = () => {
        isLightMode.update(value => !value);
        window.document.body.classList.toggle('dark-mode');
        window.document.body.style.backgroundColor = $isLightMode ? '#fff' : '#222';        
    }

    onMount(() => {
        const circle = document.createElement('div');
        circle.classList.add('color-circle');
        document.body.appendChild(circle);

        document.addEventListener('mousemove', (event) => {
            // Get mouse position
            let mouseX = event.clientX;
            let mouseY = event.clientY;

            // Set position of the circle to follow the mouse
            circle.style.left = (mouseX - 50) + 'px'; // Center the circle horizontally
            circle.style.top = (mouseY - 50) + 'px';  // Center the circle vertically

            // Calculate dynamic color based on mouse position
            let red = Math.floor((mouseX / window.innerWidth) * 255);
            let green = Math.floor((mouseY / window.innerHeight) * 255);
            let blue = 200; // Set fixed blue for contrast

            // Update the circle color
            circle.style.backgroundColor = `rgb(${red}, ${green}, ${blue})`;
        });
    });
</script>

<section class="menu">
    <div class="menu-info">
        <p class="menu-title">Paul Guerre</p>
        <p class="menu-desc">Freelance FullStack Engineer</p>
    </div>
    <div class="menu-list">
        <p on:click={() => document.getElementById("experience").scrollIntoView({ behavior: 'smooth' })}>Experience</p>
        <p on:click={() => document.getElementById("education").scrollIntoView({ behavior: 'smooth' })}>Education</p>
        <p on:click={() => document.getElementById("awards").scrollIntoView({ behavior: 'smooth' })}>Awards</p>
    </div>
    <div class="menu-theme">
        <img on:click={toggleTheme} src={$isLightMode ? moon : sun} alt="Theme logo" />
    </div>
    <div class="menu-links">
        <a href={CV_ENG} target="_blank"><img src={cv} alt="CV logo" /></a>
        <a href="mailto:contact@paulguerre.fr"><img src={mail} alt="Mail logo" /></a>
        <a href="https://github.com/PaulGuerre" target="_blank"><img src={github} alt="Github logo" /></a>
        <a href="https://www.linkedin.com/in/paul-guerre/" target="_blank"><img src={linkedin} alt="Linkedin logo" /></a>
    </div>
</section>

<style>
    .color-circle {
      position: absolute;
      width: 100px;
      height: 100px;
      border-radius: 50%;
      pointer-events: none;
      mix-blend-mode: difference;
    }

    .menu {
        width: 25vw;
        height: 100vh;
        top: 5%;
        display: flex;
        position: sticky;
        flex-direction: column;
        justify-content: start;
        gap: 20px;
    }

    .menu-title {
        font-size: 75px;
        font-weight: bold;
        margin: 0;
    }

    .menu-desc {
        font-size: 25px;
        margin: 0;
        color: #777;
    }

    .menu-theme img {
        width: 30px;
        cursor: pointer;
    }

    .menu-list {
        display: flex;
        flex-direction: column;
        align-items: start;
        justify-content: start;
        gap: 10px;

        & p {
            margin: 0;
            font-size: 20px;
            font-weight: bold;
            cursor: pointer;
            color: #128fd8;
        }
    }

    .menu-links {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: start;
        gap: 15px;

        & img {
            width: 30px;
        }
    }

    @media (max-width: 768px) {
        .menu {
            width: 100%;
            height: 100%;
            position: relative;
            top: 0;
        }

        .menu-title, .menu-desc, .menu-links, .menu-theme, .menu-list {
            padding: 5%;
        }
    }
</style>
