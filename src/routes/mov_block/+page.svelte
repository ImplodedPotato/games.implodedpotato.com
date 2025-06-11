<script lang="ts">
    // You can set the src to the path of your HTML file in the static directory
    let src = '/mov_block/mov_block.html';
</script>

<svelte:head>
    <link rel="stylesheet" href="shared.css">
</svelte:head>

<a href="../"><h2 style="position: absolute">Games.ImplodedPotato.com</h2></a>
<h1>mov_block-0.1.1</h1>

<div style="display: flex">
    <iframe title="mov_block" src={src} style="width: 80vw; height: 85vh; border: none; padding: 10px; padding-right: 15px">Galaga-Like-2D</iframe>
    <div>
        <h2>Controls:</h2>
        <p>Mouse => Move the blocks</p>
        <p>P => Play Level</p>
        <p>R => Restart Level</p>
        <p>Esc => Pause & Back</p>
    </div>
</div>



