<section class="education" id="education">
    <p class="education-main">Education</p>
    <div class="education-card">
        <p class="education-date">2021 - 2025</p>
        <div class="education-infos">
            <a href="https://www.efrei.fr/" target="_blank" class="education-title">EFREI PARIS (PARIS) 🔗</a>
            <p class="education-subtitle">Computer Science engineering degree</p>
            <p class="education-desc">Software engineering major</p>
        </div>
    </div>
    <!-- <div class="education-card">
        <p class="education-date">2024</p>
        <div class="education-infos">
            <a href="https://www.kaist.ac.kr/en/" target="_blank" class="education-title">KAIST (DAEJEON) 🔗</a>
            <p class="education-subtitle">Semester in Daejeon, organized by EFREI</p>
        </div>
    </div> -->
    <div class="education-card">
        <p class="education-date">2023</p>
        <div class="education-infos">
            <a class="education-title">Gap year (MONTREAL)</a>
            <p class="education-subtitle">First experience as a freelance developer and improvement in English</p>
        </div>
    </div>
    <div class="education-card">
        <p class="education-date">2021</p>
        <div class="education-infos">
            <a href="https://www.concordia.ca/" target="_blank" class="education-title">Concordia University (MONTREAL) 🔗</a>
            <p class="education-subtitle">Semester in Montreal, organized by EFREI</p>
        </div>
    </div>
    <div class="education-card">
        <p class="education-date">2019 - 2021</p>
        <div class="education-infos">
            <a href="https://www.u-bourgogne.fr/" target="_blank" class="education-title">IUT DE DIJON-AUXERRE (DIJON) 🔗</a>
            <p class="education-subtitle">Two-year university degree in Computer Science</p>
        </div>
    </div>
</section>

<style>
    .education {
        width: 100%;
    }

    .education-main {
        display: none;
        padding: 5%;
        font-size: 35px;
        font-weight: bold;
        color: #128fd8;
    }

    .education-card {
        display: flex;
        flex-direction: row;
        align-items: baseline;
        flex-wrap: wrap;
    }

    .education-date {
        width: 20%;
        opacity: 0.9;
    }

    .education-infos {
        width: 80%;
    }

    .education-title {
        font-size: 20px;
        font-weight: bold;
        text-decoration: none;
        cursor: pointer;
        color: #128fd8;
    }

    .education-subtitle {
        opacity: 0.9;
    }

    .education-desc {
        color: #777;
    }

    @media (max-width: 768px) {
        .education-date, .education-infos {
            width: 100%;
        }

        .education-card {
            padding: 5%;
        }

        .education-main {
            display: inline;
        }
    }
</style>
