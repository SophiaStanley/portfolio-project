<script>
    import { onMount } from 'svelte';

    onMount(() => {
        console.log("Contact Page Loaded");
    });
</script>

<h1>Contact Me</h1>
<p>Here's my college email: <a href="mailto:c00299461@setu.ie">c00299461@setu.ie</a></p>

<style>
    h1 {
        color: purple;
    }
    p {
        font-size: 18px;
    }
    a {
        color: pink;
        text-decoration: none;
    }
    a:hover {
        text-decoration: underline;
    }
</style>