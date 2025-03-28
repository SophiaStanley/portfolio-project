<script>
    import { Navigation } from "$lib";
</script>
<!-- Header -->
<header>
    <!-- logo-->
    <div class = "logo">
        <img src="/Placeholder.jpg" alt ="Website Logo">
        <h1>Sophia Stanley</h1>
    </div>

    <!--importing the header from navigation-->
    <Navigation />
</header>

<style>
    header {
        background-color: #474747;
        padding: 1rem;
        text-align: center;
    }
    .logo {
        display: flex;
        align-items: center;
    }
    .logo img {
        width: 5%;
        margin-right: 0.75rem;
    }
    h1 {
        color: white;
    }
</style>