<script>
    // Import the list of items
    import { catalogue } from '$lib/catalogue.js';
    // SvelteKit's navigation utility for client-side routing
    import { goto } from '$app/navigation';
    import { base } from '$app/paths';

    /** Function to navigate to the item's detail page
	 * @param {string} id
	 */
    function viewItem(id) {
        goto(`${base}/catalogue/${id}`);
    }
</script>


<h1>My Works</h1>

<!-- Display a grid of items -->
<div class="grid">
    {#each catalogue as item}
        <button class="card" on:click={() => viewItem(item.id)}>
            <h2>{item.title}</h2>
            <img src = '{base}{item.image}' alt = {item.alt}>
        </button>
    {/each}
</div>


<style>

    /* Unfortunately the pictures don't display fully on mobile on this page, but they do when you click into them */
    
    img {
        height: 30vh;
        align-self: center
    }
    /* Responsive grid for item layout */
    .grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
        gap: 1rem;
    }

    /* Card style for each item */
    .card {
        background: #f5f5f5;
        padding: 1rem;
        border-radius: 8px;
        cursor: pointer;
        box-shadow: 0 2px 6px rgba(0,0,0,0.1);
        transition: transform 0.2s ease;
        overflow:hidden;
        width: 100%;
        height: 90%;
    }

    .card:hover {
        transform: scale(1.05);
    }
</style>
