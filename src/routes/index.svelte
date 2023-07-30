<svelte:head>
    <title>COS Main Page</title>
</svelte:head>

<script>
    import NavigationBar from "../components/NavigationBar.svelte";
    import YoutubeVideo from "../components/YoutubeVideo.svelte";
</script>

<main>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&amp;display=swap" rel="stylesheet">
    <link rel="icon" type="image/x-icon" href="./favicon.png">

    <NavigationBar pageName="Main"/>
    <h1 class="title">Welcome to COS Software</h1>
    <div class="links">
        <a href="/videos"><button><h2>Videos</h2></button></a>
        <a href="/about"><button><h2>About COS Software</h2></button></a>
    </div>
    <div class="videos">
        <div class="recent-video">
            <h2 class="video-text">My most recent video</h2>
            <YoutubeVideo ytVidId="Drk3jVgATYA"/>
        </div>
        <div class="most-viewed-video">
            <h2 class="video-text">My most viewed video</h2>
            <YoutubeVideo ytVidId="ILJ4QVNVsIk"/>
        </div>
    </div>
</main>

<style>
  
    *{
        font-family: 'Roboto', sans-serif;
    }
    .title{
        text-align: center;
        margin: 40px;
    }
    .links{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 0 auto;
        max-width: 1200px;
        
    }   
    .videos{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 0 auto;
        max-width: 1200px;
    }
    .recent-video{
        margin: 0 auto;
        max-width: 1200px;
    }
    .most-viewed-video{
        margin: 0 auto;
        max-width: 1200px;
    }
    button{
        background-color: rgba(0, 0, 0, 0.274);
        margin: 5px;
        border: none;
        width: 200px;
        transition: all 0.3s ease-in-out;
        border-radius: 10px;
        
    }
    button:hover{
        background-color: rgba(0, 0, 0, 0.5);
        cursor: pointer;
    }
    .video-text{
        text-align: center;
    }
    @keyframes gradient {
	0% {
		background-position: 0% 50%;
	}
	50% {
		background-position: 100% 50%;
	}
	100% {
		background-position: 0% 50%;
	}
}
</style>