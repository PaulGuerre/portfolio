<script>
    import terraphore from './images/terraphore.jpg';
    import imv from './images/imv.png';
</script>

<section class="projects" id="projects">
    <div class="projects-card">
        <div class="projects-img"><img src={terraphore} alt="Terraphore image" /></div>
        <div class="projects-infos">
            <a href="https://www.efrei.fr/six-projets-davenir-pour-linnovation-day/" target="_blank" class="projects-title">Terraphore - EFREI X Bouygues Telecom 🔗</a>
            <p class="projects-desc">The Terraphore project proposes an advanced robotic reforestation system based on soil analysis. Using sensors and GPS technology, Terraphore maps the terrain, automatically selects and plants suitable trees, and monitors and maintains them. Its technical development includes a drilling system, an automated planting barrel, a soil compaction mechanism, and a watering system. By adopting an open source model, Terraphore aims to democratize reforestation by enabling global collaboration. Its sustainable business model includes the sale of kits, support services, partnerships, and diversified sources of revenue.</p>
            <div class="projects-tags">
                <p>React</p>
                <p>Typescript</p>
                <p>Docker</p>
                <p>Next.js</p>
            </div>
        </div>
    </div>
    <div class="projects-card">
        <div class="projects-img"><img src={imv} alt="Terraphore image" /></div>
        <div class="projects-infos">
            <p class="projects-title">Instagram Messages Visualizer</p>
            <p class="projects-desc">This project allows users to delve into their Instagram private messages, accessing the entire conversation history. It enables users to trace back to their first-ever messages and also explore the most recent ones. Additionally, the web application offers insightful statistics, such as message count and the date of the initial conversation. Users simply need to upload the Instagram-provided zip file and select the conversation they wish to explore.</p>
            <div class="projects-tags">
                <p>Next.js</p>
                <p>Docker</p>
            </div>
        </div>
    </div> 
</section>

<style>
    .projects {
        width: 100%;
    }
    
    .projects-card {
        display: flex;
        flex-direction: row;
        align-items: start;
        flex-wrap: wrap;
    }

    .projects-img {
        width: 20%;
        margin-top: 5%;

        & img {
            width: 80%;
            margin-top: 5px;
            border-radius: 8px;
        }
    }

    .projects-infos {
        width: 80%;
        margin-top: 5%;
    }

    .projects-title {
        font-size: 20px;
        font-weight: bold;
        text-decoration: none;
        color: #128fd8;
        cursor: pointer;
        margin: 0;
    }

    .projects-desc {
        color: #777;
    }

    .projects-tags {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 15px;
        flex-wrap: wrap;

        & p {
            background-color: #128fd8;
            color: #fff;
            font-size: 15px;
            font-weight: bold;
            border-radius: 8px;
            padding: 5px;
        }
    }

    @media (max-width: 768px) {
        .projects-img, .projects-infos {
            width: 100%;
        }

        .projects-card {
            padding: 5%;
        }
    }

    :global(body.dark-mode) .projects-tags p {
        color: #333;
    }
</style>
