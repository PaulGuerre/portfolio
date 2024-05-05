<script>
    import efrei from './images/efrei.png';
    import kaist from './images/kaist.jpg';
    import montreal from './images/montreal.jpeg';
    import concordia from './images/concordia.png';
    import iut from './images/iut.png';
</script>

<section class="education" id="education">
    <p class="education-main">Education</p>
    <div class="education-card">
        <div class="education-header">
            <p class="education-date">2021 - 2025</p>
            <div class="education-img"><img src={efrei} alt="EFREI image" /></div>
        </div>
        <div class="education-infos">
            <a href="https://www.efrei.fr/" target="_blank" class="education-title">EFREI PARIS (FRANCE) 🔗</a>
            <p class="education-subtitle">Computer Science engineering degree</p>
            <p class="education-desc">Software engineering major</p>
        </div>
    </div>
    <div class="education-card">
        <div class="education-header">
            <p class="education-date">2024</p>
            <div class="education-img"><img src={kaist} alt="KAIST image" /></div>
        </div>
        <div class="education-infos">
            <a href="https://www.kaist.ac.kr/en/" target="_blank" class="education-title">KAIST (SOUTH KOREA) 🔗</a>
            <p class="education-subtitle">Semester in Daejeon, South Korea, organized by EFREI</p>
            <p class="education-desc">Software engineering major</p>
        </div>
    </div>
    <div class="education-card">
        <div class="education-header">
            <p class="education-date">2023</p>
            <div class="education-img"><img src={montreal} alt="Montréal image" /></div>
        </div>
        <div class="education-infos">
            <a class="education-title">Gap year (CANADA)</a>
            <p class="education-subtitle">First experience as a freelance developer and improvement in English</p>
        </div>
    </div>
    <div class="education-card">
        <div class="education-header">
            <p class="education-date">2021</p>
            <div class="education-img"><img src={concordia} alt="Concordia image" /></div>
        </div>
        <div class="education-infos">
            <a href="https://www.concordia.ca/" target="_blank" class="education-title">Concordia University (CANADA) 🔗</a>
            <p class="education-subtitle">Semester in Montreal, organized by EFREI</p>
            <p class="education-desc">Software engineering major</p>
        </div>
    </div>
    <div class="education-card">
        <div class="education-header">
            <p class="education-date">2019</p>
            <div class="education-img"><img src={iut} alt="IUT image" /></div>
        </div>
        <div class="education-infos">
            <a href="https://www.u-bourgogne.fr/" target="_blank" class="education-title">IUT DE DIJON-AUXERRE (FRANCE) 🔗</a>
            <p class="education-subtitle">Two-year university degree in Computer Science</p>
            <p class="education-desc">Long study programm</p>
        </div>
    </div>
</section>

<style>
    .education {
        width: 100%;
        margin-bottom: 75px;
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
        margin-bottom: 25px;
    }

    .education-header {
        width: 20%;
        text-align: center;
    }

    .education-img img {
        border: 2px solid #128fd8;
        width: 50%;
        border-radius: 50px;
    }

    .education-date {
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
        .education-card {
            padding: 5%;
        }

        .education-main {
            display: inline;
        }
    }
</style>
