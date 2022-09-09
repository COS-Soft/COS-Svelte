<svelte:head>
    <title>COS About Page</title>
</svelte:head>

<script>
    import NavigationBar from "../components/NavigationBar.svelte";
</script>

<main>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&amp;display=swap" rel="stylesheet">
    <NavigationBar pageName="About" />

    <div>
        <h1>About COS Software</h1>
        <p>"COS" actually means Computers and Operating Systems. </p>
        <p>I do a lot of projects about computers. And every now and then I upload a video about a project I made.</p>
        <p>This channel was created in March 13, 2020.</p>
        <p>Here is a link to my YouTube channel: <a href="https://www.youtube.com/channel/UCWcOyUE0eTUACW-QhhQ76SA">https://www.youtube.com/channel/UCWcOyUE0eTUACW-QhhQ76SA</a></p>
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
    /* Roboto Font*/
    *{
        font-family: 'Roboto', sans-serif;
    }
    div{
        margin: 10px;
    }
    p{
        font-size: 1.2rem;
    }
</style>