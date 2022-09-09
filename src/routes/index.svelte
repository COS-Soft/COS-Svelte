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
            <YoutubeVideo ytVidId="ESmnRvZdt5w"/>
        </div>
        <div class="most-viewed-video">
            <h2 class="video-text">My most viewed video</h2>
            <YoutubeVideo ytVidId="ILJ4QVNVsIk"/>
        </div>
    </div>
</main>

<style>
    main {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: -1;
}

main:after, main:before {
  position: absolute;
  top: 0;
  left: 0;
  width: 400%;
  height: 400%;
  content: "";
  z-index: -1;
}

main:after {
  background: radial-gradient(circle, red, transparent);
  animation: colorSpin 30s linear infinite;
}

main:before {
  background-color: yellow;
}

@keyframes colorSpin {
  25% {
    transform: translateY(-75%);
  }
  50% {
    transform: translate(-75%, -75%);
  }
  75% {
    transform: translate(-75%, 0);
  }
  100% {
    filter: hue-rotate(360deg);
  }
  /*75 is obtained as 100[1- (100/(height or width written in main:after)). i.e. 75 = 100[1-100/400] */
}
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
        background-color: rgb(218, 218, 218);
        margin: 5px;
        border: none;
        width: 200px;
        transition: all 0.3s ease-in-out;
        border-radius: 10px;
    }
    button:hover{
        background-color: rgb(56, 56, 56);
        color: white;
    }
    .video-text{
        text-align: center;
    }
</style>