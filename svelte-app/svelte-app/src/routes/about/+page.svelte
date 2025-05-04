<script>
    import { onMount } from 'svelte';

    onMount(() => {
        console.log("About Page Loaded");
    });
</script>

<div class = "about">
    <h1>About Me</h1>
    <p>I am an artist specialising in illustration and concept art. I currently attend South East Technological University Carlow
    and am studying Computing in Interactive Digital Art and Design. I also do some UI and UX design. I coded this website! :D</p>
</div>


<style>
    div {
        margin-top: 1%; 
        background-color: #CEC2FF;
        height: 60vh;
        width: 60vw;
        position: absolute;
        justify-content: right;
        padding-left: 5vw;
        padding-right: 5vw;
        align-self: center;
    }
    h1 {
        margin-top: 20vh;
    }
</style>