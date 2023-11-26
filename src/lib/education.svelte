<section class="education">
    <div class="education-card" id="education">
        <p class="education-date">2021 - 2024</p>
        <div class="education-infos">
            <a href="https://www.efrei.fr/" target="_blank" class="education-title">EFREI PARIS (PARIS) 🔗</a>
            <p class="education-subtitle">Computer Science engineering degree</p>
            <p class="education-desc">Software engineering major</p>
        </div>
    </div>
    <div class="education-card">
        <p class="education-date">2021</p>
        <div class="education-infos">
            <a href="https://www.concordia.ca/" target="_blank" class="education-title">Concordia University (MONTREAL) 🔗</a>
            <p class="education-subtitle">Semester in Montreal, organized by EFREI</p>
            <p class="education-desc">Web, OS, Hardware, Networks, POO, UML, JAVA</p>
        </div>
    </div>
    <div class="education-card">
        <p class="education-date">2019 - 2021</p>
        <div class="education-infos">
            <a href="https://www.u-bourgogne.fr/" target="_blank" class="education-title">IUT DE DIJON-AUXERRE (DIJON) 🔗</a>
            <p class="education-subtitle">Two-year university degree in Computer Science</p>
            <p class="education-desc">Algo, Web, POO, COO, UML, AI, System, Networks, DB</p>
        </div>
    </div>
</section>

<style>
    .education {
        width: 100%;
    }

    .education-card {
        display: flex;
        flex-direction: row;
        align-items: baseline;
        flex-wrap: wrap;
    }

    .education-date {
        width: 20%;
        opacity: 0.7;
    }

    .education-infos {
        width: 80%;
    }

    .education-title {
        font-size: 20px;
        font-weight: bold;
        text-decoration: none;
        cursor: pointer;
        color: #00FF00;
    }

    .education-subtitle {
        opacity: 0.5;
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
    }
</style>
