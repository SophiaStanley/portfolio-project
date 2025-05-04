<script>
    // `data` is automatically provided by the load function from +page.js
    export let data;

    // Bring in the navigation helper
    import { goto } from '$app/navigation';

    // Destructure item from the loaded data
    const { item } = data;
</script>


<!-- Back button -->
<button on:click={() => goto('/catalogue')}>← Back to Catalogue</button>

<!-- Display item details -->
<h1>{item.title}</h1>
<img src = {item.image} alt = {item.alt}>
<p>{item.description}</p>


<style>
    button {
        margin-bottom: 1rem;
        background-color: rgb(171, 22, 205);
        color: white;
        padding: 0.5rem 1rem;
        border-radius: 6px;
        border: none;
        cursor: pointer;
    }

    button:hover {
        background-color: rgb(149, 0, 183);
    }

    img {
        height: 20%;
        width: 50%;
        align-self: center;
    }
    p {
        padding-bottom: 5vh;
    }
    @media (max-width: 768px) {
        img {
            height: 30%;
            width: 100%;
        }
    }
</style>
  