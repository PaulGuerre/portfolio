<script>
    import js from './images/js.png';
    import node from './images/node.png';
    import next from './images/next.png';
    import react from './images/react.png';
    import vue from './images/vue.png';
    import svelte from './images/svelte.png';
    import sql from './images/sql.png';
    import mariadb from './images/mariadb.png';
    import mysql from './images/mysql.png';
    import docker from './images/docker.png';
    import linux from './images/linux.png';
    import scrum from './images/scrum.png';
</script>

<section class="skills" id="skills">
    <p class="skills-main">Skills</p>
    <div class="skills-container">
        <div class="skills-card">
            <img src={js} alt="JS image" />
            <p class="skills-title">Javascript</p>
        </div>
        <div class="skills-card">
            <img src={node} alt="Node.JS image" />
            <p class="skills-title">Node.JS</p>
        </div>
        <div class="skills-card">
            <img src={next} alt="Next.JS image" />
            <p class="skills-title">Next.JS</p>
        </div>
        <div class="skills-card">
            <img src={react} alt="React.JS image" />
            <p class="skills-title">React.JS</p>
        </div>
        <div class="skills-card">
            <img src={vue} alt="Vue.JS image" />
            <p class="skills-title">Vue.JS</p>
        </div>
        <div class="skills-card">
            <img src={svelte} alt="Svelte image" />
            <p class="skills-title">Svelte</p>
        </div>
        <hr class="separator" />
        <div class="skills-card">
            <img src={sql} alt="SQL image" />
            <p class="skills-title">SQL</p>
        </div>
        <div class="skills-card">
            <img src={mariadb} alt="MariaDB image" />
            <p class="skills-title">MariaDB</p>
        </div>
        <div class="skills-card">
            <img src={mysql} alt="MySQL image" />
            <p class="skills-title">MySQL</p>
        </div>
        <hr class="separator" />
        <div class="skills-card">
            <img src={docker} alt="Docker image" />
            <p class="skills-title">Docker</p>
        </div>
        <div class="skills-card">
            <img src={linux} alt="Linux image" />
            <p class="skills-title">Linux</p>
        </div>
        <hr class="separator" />
        <div class="skills-card">
            <img src={scrum} alt="Scrum image" />
            <p class="skills-title">Scrum</p>
        </div>
    </div>
</section>

<style>
    .skills {
        width: 100%;
        margin-bottom: 75px;
    }

    .skills-main {
        padding: 5% 5% 0 5%;
        font-size: 35px;
        font-weight: bold;
        color: #128fd8;
    }

    .skills-container {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        margin-bottom: 25px;
        padding-left: 5%;
        gap: 5%;
    }

    .skills-card {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        gap: 15px;
        padding: 2%;
    }

    .separator {
        width: 100%;
        border: 1px solid #128fd8;
        margin: 25px 0;
    }

    .skills-card img {
        border: 2px solid #128fd8;
        width: 50px;
        border-radius: 50px;
    }

    .skills-title {
        font-size: 20px;
        font-weight: bold;
        text-decoration: none;
        color: #128fd8;
    }

    @media (max-width: 768px) {
        .skills-container {
            padding: 5%;
        }

        .skills-main {
            display: inline;
        }
    }
</style>
