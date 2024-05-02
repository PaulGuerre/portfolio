<script>
    import kameo from './images/kameo.jpg';
    import sukine from './images/sukine.jpeg';
</script>

<section class="clients" id="clients">
    <p class="clients-main">Clients</p>
    <div class="clients-card">
        <div class="clients-img"><img src={kameo} alt="Kameo company logo" /></div>
        <div class="clients-infos">
            <a href="https://agence-kameo.fr/" target="_blank" class="clients-title">Agence Kameo 🔗</a>
            <p class="clients-desc">Web development & DIGITAL MARKETING</p>
        </div>
    </div>
    <div class="clients-card">
        <div class="clients-img"><img src={sukine} alt="Sukine company logo" /></div>
        <div class="clients-infos">
            <a class="clients-title">Sukine Corporation</a>
            <p class="clients-desc">Creation and development of projects of all kinds</p>
        </div>
    </div>
</section>

<style>
    .clients {
        width: 100%;
    }

    .clients-main {
        display: none;
        padding: 5%;
        font-size: 35px;
        font-weight: bold;
        color: #128fd8;
    }

    .clients-card {
        display: flex;
        flex-direction: row;
        align-items: start;
        flex-wrap: wrap;
    }
    
    .clients-img {
        width: 20%;
        text-align: center;
    
        & img {
            border: 2px solid #128fd8;
            width: 50%;
            margin: 25px;
            border-radius: 50px;
        }
    }
    
    .clients-infos {
        width: 80%;
        margin-top: 5%;
    }
    
    .clients-title {
        font-size: 20px;
        font-weight: bold;
        margin-top: 25px;
        cursor: pointer;
        text-decoration: none;
        color: #128fd8;
    }
    
    .clients-desc {
        color: #777;
    }

    @media (max-width: 768px) {
        .clients-img {
            text-align: center;
        }

        .clients-img img {
            margin: 25px 0;
        }

        .clients-card {
            padding: 5%;
        }

        .clients-main {
            display: inline;
        }
    }
</style>    
