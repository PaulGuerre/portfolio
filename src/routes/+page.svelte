<script>
  import Awards from "$lib/awards.svelte";
  import Clients from "$lib/clients.svelte";
  import Education from "$lib/education.svelte";
  import Experience from "$lib/experience.svelte";
  import Menu from "$lib/menu.svelte";
  import Projects from "$lib/projects.svelte";
</script>

<svelte:head>
	<title>Paul Guerre</title>
	<meta name="description" content="Freelance software engineer and full-stack developer, showcasing a diverse portfolio of innovative projects. Explore my educational background, professional experience, and client testimonials. Your go-to for transforming ideas into robust software solutions.">
</svelte:head>

<section class="app">
    <div class="main">
        <Menu />
        <div class="main-data">
            <Experience />
            <Education />
            <Projects />
            <Awards />
            <Clients />
        </div>
    </div>
</section>

<style>
    .app {
        display: grid;
        width: 100%;
        background-color: #fff;
        font-family: 'Roboto', sans-serif;
        color: #128fd8;
    }

    .main {
        width: 75vw;
        justify-self: center;
        align-self: center;
        display: flex;
        flex-direction: row;
        justify-content: center;
        gap: 150px;
    }

    .main-data {
        width: 50vw;
        margin: 20px 0;
        display: flex;
        flex-direction: column;
        align-items: start;
        justify-content: center;
    }

    @media (max-width: 768px) {
        .main {
            flex-direction: column;
            width: 100%;
        }

        .main-data {
            width: 100%;
        }
    }

    :global(body.dark-mode) .app {
        background-color: #222;
    }
</style>
