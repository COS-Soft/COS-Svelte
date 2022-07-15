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
        <p>This channel was created in March 13, 2020 and since then this channel changed a lot.</p>
        <p>Here is a link to my YouTube channel: <a href="https://www.youtube.com/channel/UCWcOyUE0eTUACW-QhhQ76SA">https://www.youtube.com/channel/UCWcOyUE0eTUACW-QhhQ76SA</a></p>
    </div>
</main>

<style>    
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