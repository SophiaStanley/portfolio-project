<script>
    import { onMount } from 'svelte';

    onMount(() => {
        console.log("Home Page Loaded");
    });
</script>

<div>
    <h1>Sophia Stanley</h1>
    <p>Concept Artist</p>
    <br>
    <p><a href="/works">View Work</a></p>
</div>

<img src=/HomeImage.png alt = "Selt Portrait">

<style>
    /* There's a lot of responsiveness issues right now */
    div {
        margin-top: 5%;
        background-color: rgb(176, 0, 215);
        height: 50vh;
        width: 60vw;
        position: absolute;
    }
    h1 {
        margin-top: 15vh;
    }
    a {
        background-color: purple;
        padding: 10px;
    }
    a:hover {
        background-color: rgb(49, 0, 60)
    }

    img {
        position:relative;
        height: 609px;
        width: 421px;
        margin-left: 60vw;
    }
    
</style>