<svelte:head>
    <title>COS Courses</title>
</svelte:head>

<script>
    import NavigationBar from "../components/NavigationBar.svelte";
    import Course from "../components/Course.svelte";
</script>

<main>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">

    <NavigationBar pageName="Courses"/>

    <div class="courses">
        <h1>Coming Soon!</h1>
        <Course courseID="COS 126"/>
    </div>
</main>

<style>
    *{
        font-family: 'Roboto', sans-serif;
    }
    .courses{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 0 auto;
        max-width: 1200px;
    }
</style>