<script>
    import sopraSteria from './images/sopraSteria.png';
    import kmb from './images/kmb.jpg';
    import satisfactory from './images/satisfactory.jpeg';
</script>

<section class="experience" id="experience">
    <p class="experience-main">Experience</p>
    <div class="experience-card">
        <div class="experience-header">
            <p class="experience-date">2025 - present</p>
            <div class="projects-img"><img src={sopraSteria} alt="Sopra Steria image" /></div>
        </div>
        <div class="experience-infos">
            <a href="https://www.soprasteria.com/" target="_blank" class="experience-title">SOPRA STERIA (PARIS) 🔗</a>
            <p class="experience-subtitle">Fullstack developer</p>
        </div>
    </div>
    <div class="experience-card">
        <div class="experience-header">
            <p class="experience-date">2022 - 2023</p>
            <div class="projects-img"><img src={kmb} alt="KMB image" /></div>
        </div>
        <div class="experience-infos">
            <a href="https://www.kmblabs.com/" target="_blank" class="experience-title">KMB LABS (PARIS) 🔗</a>
            <p class="experience-subtitle">Fullstack developer</p>
            <div class="experience-tags">
                <p>React</p>
                <p>Javascript</p>
                <p>Docker</p>
            </div>
        </div>
    </div>
    <div class="experience-card">
        <div class="experience-header">
            <p class="experience-date">2021</p>
            <div class="projects-img"><img src={satisfactory} alt="Satisfactory image" /></div>
        </div>
        <div class="experience-infos">
            <a href="https://www.satisfactory.fr/" target="_blank" class="experience-title">SATISFACTORY (PARIS) 🔗</a>
            <p class="experience-subtitle">Frontend developer</p>
            <div class="experience-tags">
                <p>Angular</p>
                <p>Symfony</p>
                <p>Docker</p>
            </div>
        </div>
    </div>
</section>

<style>
    .experience {
        width: 100%;
        margin-bottom: 50px;
    }

    .experience-main {
        padding: 5% 5% 0 5%;
        font-size: 35px;
        font-weight: bold;
        color: #128fd8;
    }

    .experience-card {
        display: flex;
        flex-direction: row;
        align-items: baseline;
        flex-wrap: wrap;
        margin-bottom: 25px;
    }

    .experience-header {
        width: 20%;
        text-align: center;
    }

    .projects-img img {
        border: 2px solid #128fd8;
        width: 50%;
        border-radius: 50px;
    }

    .experience-date {
        opacity: 0.9;
    }

    .experience-infos {
        width: 80%;
    }

    .experience-title {
        font-size: 20px;
        font-weight: bold;
        text-decoration: none;
        cursor: pointer;
        color: #128fd8;
    }

    .experience-subtitle {
        opacity: 0.9;
    }

    .experience-tags {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 15px;
        flex-wrap: wrap;

        & p {
            margin: 0;
            background-color: #128fd8;
            color: #222;
            font-size: 15px;
            font-weight: bold;
            border-radius: 8px;
            padding: 5px;
        }
    }

    @media (max-width: 768px) {
        .experience-card {
            padding: 5%;
        }

        .experience-main {
            display: inline;
        }
    }

    :global(body.dark-mode) .experience-tags p {
        color: #fff;
    }
</style>
