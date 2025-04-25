<script>
    import { onMount } from 'svelte';

    onMount(() => {
        console.log("About Page Loaded");
    });
</script>

<h1>About Me</h1>
<p>I go to college and do other things sometimes</p>

<br>

<h1>Contact Me</h1>
<p>Here's my college email: <a href="mailto:c00299461@setu.ie">c00299461@setu.ie</a></p>

<style>
    h1 {
        color: purple;
    }
    p {
        font-size: 18px;
    }
</style>