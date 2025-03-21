<script>
    import { onMount } from 'svelte';

    onMount(() => {
        console.log("About Page Loaded");
    });
</script>

<h1>About Me</h1>
<p>I go to college and do other things sometimes</p>

<style>
    h1 {
        color: purple;
    }
    p {
        font-size: 18px;
    }
</style>