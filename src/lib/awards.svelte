<script>
    import bouygues from './images/bouygues.png';
</script>

<section class="awards" id="awards">
    <p class="awards-main">Awards</p>
    <div class="awards-card">
        <div class="awards-header">
            <p class="awards-date">2023</p>
            <div class="awards-img"><img src={bouygues} alt="Bouygues Telecom image" /></div>
        </div>
        <div class="awards-infos">
            <a href="https://www.efrei.fr/six-projets-davenir-pour-linnovation-day/" target="_blank" class="awards-title">1ST PRIZE INNOVATION DAY EFREI</a>
            <p class="awards-subtitle">Efrei paris and Bouygues Telecom</p>
            <p class="awards-desc">Winning the first prize at the Efrei innovation day, by presenting the POC (proof of concept) of a tree-planting robot.</p>
        </div>
    </div>
</section>

<style>
    .awards {
        width: 100%;
        margin-bottom: 50px;
    }

    .awards-main {
        padding: 5% 5% 0 5%;
        font-size: 35px;
        font-weight: bold;
        color: #128fd8;
    }

    .awards-card {
        display: flex;
        flex-direction: row;
        align-items: baseline;
        flex-wrap: wrap;
        margin-bottom: 25px;
    }

    .awards-header {
        width: 20%;
        text-align: center;
    }

    .awards-img img {
        border: 2px solid #128fd8;
        width: 50%;
        border-radius: 50px;
    }

    .awards-date {
        opacity: 0.9;
    }

    .awards-infos {
        width: 80%;
    }

    .awards-title {
        font-size: 20px;
        font-weight: bold;
        text-decoration: none;
        cursor: pointer;
        color: #128fd8;
    }

    .awards-subtitle {
        opacity: 0.9;
    }

    .awards-desc {
        color: #777;
    }

    @media (max-width: 768px) {
        .awards-card {
            padding: 5%;
        }

        .awards-main {
            display: inline;
        }
    }
</style>
