<script>
    import terraphore from './images/terraphore.jpg';
    import sukify from './images/sukify.png';
    import imv from './images/imv.png';
    import onlyvote from './images/onlyvote.png';
    import wol from './images/wol.png';
    import arch from './images/arch.png';
</script>

<section class="projects" id="projects">
    <p class="projects-main">Projects</p>
    <div class="projects-card">
        <div class="projects-infos">
            <a href="https://www.efrei.fr/six-projets-davenir-pour-linnovation-day/" target="_blank" class="projects-title">Terraphore - EFREI X Bouygues Telecom 🔗</a>
            <div class="projects-img"><img src={terraphore} alt="Terraphore image" /></div>
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
        <div class="projects-infos">
            <a href="https://github.com/PaulGuerre/sukify-v2" target="_blank" class="projects-title">Sukify 🔗</a>
            <div class="projects-img"><img src={sukify} alt="Sukify image" /></div>
            <p class="projects-desc">Sukify is a private music web server that allows you to add and listen to music from Youtube. The web platform lets you download music and create playlists. About the music player, you have the option to enable shuffle music mode or music repeat mode. It uses the Youtube API.</p>
            <div class="projects-tags">
                <p>React</p>
                <p>Docker</p>
                <p>Next.js</p>
                <p>Express</p>
            </div>
        </div>
    </div>
    <div class="projects-card">
        <div class="projects-infos">
            <a href="https://github.com/PaulGuerre/IMV" target="_blank" class="projects-title">Instagram Messages Visualizer 🔗</a>
            <div class="projects-img"><img src={imv} alt="IMV image" /></div>
            <p class="projects-desc">This project allows users to delve into their Instagram private messages, accessing the entire conversation history. It enables users to trace back to their first-ever messages and also explore the most recent ones. Additionally, the web application offers insightful statistics, such as message count and the date of the initial conversation. Users simply need to upload the Instagram-provided zip file and select the conversation they wish to explore.</p>
            <div class="projects-tags">
                <p>Next.js</p>
                <p>Docker</p>
            </div>
        </div>
    </div> 
    <div class="projects-card">
        <div class="projects-infos">
            <a href="https://github.com/PaulGuerre/OnlyVote/tree/android-app" target="_blank" class="projects-title">OnlyVote 🔗</a>
            <div class="projects-img"><img src={onlyvote} alt="OnlyVote image" /></div>
            <p class="projects-desc">This project is a comprehensive voting platform for important elections. I developed the Android app, which supports both light and dark modes. The app allows users to read about election programs, register using phone number authentication, and vote for their preferred candidate. This project has been a valuable part of my journey as a developer.</p>
            <div class="projects-tags">
                <p>Node.js</p>
                <p>Kotlin</p>
            </div>
        </div>
    </div> 
    <div class="projects-card">
        <div class="projects-infos">
            <a href="https://github.com/PaulGuerre/Wake-On-Lan-Lite" target="_blank" class="projects-title">Wake On Lan Lite 🔗</a>
            <div class="projects-img"><img src={wol} alt="Wake On Lan Lite image" /></div>
            <p class="projects-desc">This project is a simple Wake On Lan software that enables waking up a computer on your local network. Users can add devices to a list and choose to wake them up as needed. The software requires the name and MAC address of the device. This project has provided me with practical experience in network programming.</p>
            <div class="projects-tags">
                <p>C#</p>
                <p>Network</p>
            </div>
        </div>
    </div> 
    <div class="projects-card">
        <div class="projects-infos">
            <a href="https://github.com/PaulGuerre/arch_dotfiles" target="_blank" class="projects-title">Archlinux dotfiles 🔗</a>
            <div class="projects-img"><img src={arch} alt="Archlinux image" /></div>
            <p class="projects-desc">This project is my custom Archlinux dotfiles. It uses Archlinux as the OS, Hyprland for window management, Grub-silent and Plymouth for a clean and animated boot process, and Ly for fast login. The shell is Zsh with Starship, and the terminal is Alacritty. The bar is Waybar, the notify daemon is Mako (now swaync), and the menu is Wofi. The lock screen is a custom fork of Swaylock called Swaylock-effects-text, which allows for text customization. The wallpaper handler is Oguri, which supports GIFs. Other features include a Spotify theme via Spicetify, a Dracula GTK theme, and the SourceCodePro font. This project has been a significant part of my journey in customizing Linux environments.</p>
            <div class="projects-tags">
                <p>Shell</p>
                <p>C</p>
                <p>CSS</p>
            </div>
        </div>
    </div> 
</section>

<style>
    .projects {
        width: 100%;
        margin-bottom: 75px;
    }

    .projects-main {
        padding: 5% 5% 0 5%;
        font-size: 35px;
        font-weight: bold;
        color: #128fd8;
    }
    
    .projects-card {
        display: flex;
        flex-direction: row;
        align-items: start;
        flex-wrap: wrap;
        margin-left: 5%;
    }

    .projects-img {
        margin-top: 5%;

        & img {
            width: 80%;
            margin-top: 5px;
            border-radius: 8px;
        }
    }

    .projects-infos {
        margin-top: 5px;
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
        .projects-card {
            padding: 5%;
        }

        .projects-main {
            display: inline;
        }
    }

    :global(body.dark-mode) .projects-tags p {
        color: #222;
    }
</style>
