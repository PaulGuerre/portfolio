<script>
    import mail from '../lib/images/mail.svg';
    import github from '../lib/images/github.svg';
    import linkedin from '../lib/images/linkedin.svg';
    import sun from '../lib/images/sun.svg';
    import moon from '../lib/images/moon.svg';
    import { writable } from 'svelte/store';

    const isDarkMode = writable(false);

    const toggleTheme = () => {
        isDarkMode.update(value => !value);
        window.document.body.classList.toggle('dark-mode');
        window.document.body.style.backgroundColor = $isDarkMode ? '#333' : '#fff';
    }
</script>

<section class="menu">
    <div class="menu-info">
        <p class="menu-title">Paul Guerre</p>
        <p class="menu-desc">Freelance FullStack Engineer</p>
    </div>
    <div class="menu-list">
        <p on:click={() => document.getElementById("experience").scrollIntoView({ behavior: 'smooth' })}>Experience</p>
        <p on:click={() => document.getElementById("education").scrollIntoView({ behavior: 'smooth' })}>Education</p>
        <p on:click={() => document.getElementById("projects").scrollIntoView({ behavior: 'smooth' })}>Projects</p>
        <p on:click={() => document.getElementById("clients").scrollIntoView({ behavior: 'smooth' })}>Clients</p>
    </div>
    <div class="menu-theme">
        <img on:click={toggleTheme} src={$isDarkMode ? sun : moon} alt="Theme logo" />
    </div>
    <div class="menu-links">
        <a href="mailto:contact@paulguerre.fr"><img src={mail} alt="Mail logo" /></a>
        <a href="https://github.com/Paulobergine" target="_blank"><img src={github} alt="Github logo" /></a>
        <a href="https://www.linkedin.com/in/paul-guerre/" target="_blank"><img src={linkedin} alt="Linkedin logo" /></a>
    </div>
</section>

<style>
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
