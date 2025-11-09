<script lang="ts">
    // You can set the src to the path of your HTML file in the static directory
    let src = '/cand/cand.html';
</script>

<svelte:head>
    <link rel="stylesheet" href="shared.css">
</svelte:head>

<a href="../"><h2 style="position: absolute">Games.ImplodedPotato.com</h2></a>
<h1>cand</h1>

<div style="display: flex; margin-left: 50px;">
    <iframe title="cand" src={src} style="width: calc(800px + 364px); height: calc(600px + 16px); border: none; padding: 10px;">cand</iframe>
    <div style="align-items: center; margin-left: 50px;">
        <div>
            <h2>Controls:</h2>
            <p>R => Reset</p>
            <p>G => Toggle Grid Lines </p>
            <p>Click => Place Sand </p>
        </div>

        <div style="margin-top: 100px;">
            <h2>Details:</h2>
            <a href="https://github.com/implodedPotato/cand">GitHub</a>
            <p>Made in C with <a href="https://www.raylib.com/">Raylib</a></p>
            <p>A simple sand and liquid simulator</p>
        </div>
    </div>
</div>
<style>

</style>
