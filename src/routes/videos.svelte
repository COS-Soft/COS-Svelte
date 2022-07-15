<svelte:head>
    <title>COS Videos Page</title>
</svelte:head>

<script>
    import NavigationBar from "../components/NavigationBar.svelte";
    import YoutubeVideo from "../components/YoutubeVideo.svelte";
</script>

<main>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&amp;display=swap" rel="stylesheet">

    <NavigationBar pageName="Videos"/>

    <div class="videos">
        <YoutubeVideo ytVidId="ESmnRvZdt5w"/>
        <YoutubeVideo ytVidId="ILJ4QVNVsIk"/>
        <YoutubeVideo ytVidId="EyPkj3OVbBA"/>
        <YoutubeVideo ytVidId="f5jpzzh6GxU"/>
        <YoutubeVideo ytVidId="VeG-zHyyEEU"/>
        <YoutubeVideo ytVidId="b7RcDjOc3T0"/>
        <YoutubeVideo ytVidId="gIo58Qy-Jl0"/>
        <YoutubeVideo ytVidId="8ZPnHyCcLYQ"/>
        <YoutubeVideo ytVidId="QEE8N7YpKnc"/>
        <YoutubeVideo ytVidId="oDmvouS1r6A"/>
        <YoutubeVideo ytVidId="wIyAnYu22oU"/>
    </div>

</main>

<style>
    *{
        font-family: 'Roboto', sans-serif;
    }
    .videos{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 0 auto;
        max-width: 1200px;
    }
</style>