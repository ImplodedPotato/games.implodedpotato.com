<script lang="ts">
    // You can set the src to the path of your HTML file in the static directory
    let src = '/Galaga-Like-2D/Galaga-Like-2D.html';
</script>

<svelte:head>
    <link rel="stylesheet" href="shared.css">
</svelte:head>

<a href="../"><h2 style="position: absolute">Games.ImplodedPotato.com</h2></a>
<h1>Galaga-Like-2D</h1>

<div style="display: flex">
    <iframe title="Galaga-Like-2D" src={src} style="width: 80vw; height: 85vh; border: none; padding: 10px; padding-right: 15px">Galaga-Like-2D</iframe>
    <div>
        <h2>Controls:</h2>
        <p>WASD => Up/Left/Down/Right</p>
        <p>Arrow Keys => Up/Left/Down/Right</p>
        <p>Space => Shoot</p>
        <p>Return => Restart When Dead</p>
        <p>Tilde => Show Hitboxes</p>
    </div>
</div>