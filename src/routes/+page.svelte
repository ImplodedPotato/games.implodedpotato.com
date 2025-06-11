<script lang="ts">
    let buttons = [
        {
            h1: "ImplodedPotato.com",
            h2: "The main site",
            link: "https://implodedpotato.com"
        },
        {
            h1: "Galaga-like-2D",
            h2: "Made in C with Raylib",
            link: "/Galaga-Like-2D"
        },
        {
            h1: "Galaga-like-3D",
            h2: "Made in C++ with Raylib",
            link: "/Galaga-Like-3D"
        },
        {
            h1: "Simple Physics Sim",
            h2: "Made in Rust with Raylib",
            link: "/PhySim"
        },
        {
            h1: "mov_block-0.1.1",
            h2: "Made in bevy for the 6th bevy Jam",
            link: "/mov_block"
        },
    ]
</script>

<svelte:head>
    <link rel="preload" as="font" href="/FiraCode-Retina.ttf" type="font/ttf" crossorigin="anonymous">
    <link rel="stylesheet" href="shared.css">
</svelte:head>

<h1>Welcome to Games.ImplodedPotato.com</h1>
<p>Here you will find the 'many' games of a Potato which has been Imploded</p>

<div class="main-buttons-capsule">
    {#each buttons as button (button.link)}
        <a href="{button.link}">
            <div class="main-buttons">
                <p>{button.h1}</p>
                <p style="margin-top: 10px; margin-bottom: 50px">{button.h2}</p>
            </div>
        </a>
    {/each}
</div>

<a href="https://github.com/ImplodedPotato/games.implodedpotato.com/">
    <img style="position: fixed; bottom: 8px; right: 8px; scale: 0.6" src="github-mark-white.svg" alt="GitHub">
</a>

<style>
    .main-buttons-capsule {
        padding-top: 5vh;
        display: grid;
        grid-template-columns: repeat(auto-fill, min-content);
        gap: 10px;
        margin: auto;
        max-width: max-content;
    }

    @media screen and (min-width: 600px) {
        .main-buttons-capsule {
            grid-template-columns: repeat(2, min-content);
        }
    }

    @media screen and (min-width: 900px) {
        .main-buttons-capsule {
            grid-template-columns: repeat(3, min-content);
        }
    }

    .main-buttons {
        background-color: #49485e;
        padding: 5px;
        border-radius: 10px;
        display: block;
        width: 250px;
        height: 250px;
        font-size: medium;
        align-content: center;
    }

    .main-buttons:hover {
        background-color: #54617e;
    }

    a {
        color: aquamarine;
        text-decoration: none;
    }
</style>