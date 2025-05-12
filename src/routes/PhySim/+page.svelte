<script lang="ts">
    // You can set the src to the path of your HTML file in the static directory
    let src = '/PhySim/PhySim.html';
</script>

<svelte:head>
    <link rel="stylesheet" href="shared.css">
</svelte:head>

<a href="../"><h2 style="position: absolute">Games.ImplodedPotato.com</h2></a>
<h1>PhySim</h1>

<div style="display: flex">
    <iframe title="PhySim" src={src} style="width: 80vw; height: 85vh; border: none; padding: 10px; padding-right: 15px">PhySim</iframe>
    <div>
        <h2>Controls:</h2>
        <p>R => Restart</p>
        <p>A => Move Left</p>
        <p>D => Move Right</p>
        <p>W => Jump Up</p>
        <p>S => Slam Up</p>
    </div>
</div>
<style>
    :global {
        iframe {

        }

    }

</style>



