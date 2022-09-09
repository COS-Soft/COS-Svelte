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
    .videos{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 0 auto;
        max-width: 1200px;
    }
</style>