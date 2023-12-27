<section class="experience" id="experience">
    <p class="experience-main">Experience</p>
    <div class="experience-card">
        <p class="experience-date">2022 - 2023</p>
        <div class="experience-infos">
            <a href="https://www.kmblabs.com/" target="_blank" class="experience-title">KMB LABS (PARIS) 🔗</a>
            <p class="experience-subtitle">Fullstack developer</p>
            <p class="experience-desc">Participation and development of the company's products: chatbots, search engines, backoffice and other web services. Participation in the reflection on the logical and material architecture. Work on different technologies such as Node.js, React, GraphQL, Docker, serverless....</p>
        </div>
    </div>
    <div class="experience-card">
        <p class="experience-date">2021</p>
        <div class="experience-infos">
            <a href="https://www.satisfactory.fr/" target="_blank" class="experience-title">SATISFACTORY (PARIS) 🔗</a>
            <p class="experience-subtitle">Fullstack developer</p>
            <p class="experience-desc">Development and maintenance of the company's web platform, which is its main product, within a team operating according to the principle of agility, on Angular, Symfony and Docker technologies</p>
        </div>
    </div>
</section>

<style>
    .experience {
        width: 100%;
    }

    .experience-main {
        display: none;
        padding: 5%;
        font-size: 35px;
        font-weight: bold;
        color: #128fd8;
    }

    .experience-card {
        display: flex;
        flex-direction: row;
        align-items: baseline;
        flex-wrap: wrap;
    }

    .experience-date {
        width: 20%;
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

    .experience-desc {
        color: #777;
    }

    @media (max-width: 768px) {
        .experience-date, .experience-infos {
            width: 100%;
        }

        .experience-card {
            padding: 5%;
        }

        .experience-main {
            display: inline;
        }
    }
</style>
