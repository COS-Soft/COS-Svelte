<script>
    export let ytVidId = ''; 
    let vidElementIdName = `video${ytVidId}`;
    //console.log(ytVidId);

    function playVid(){
        let vid = document.getElementById(vidElementIdName);
        vid.style.opacity = '1';
        vid.style.pointerEvents = 'auto';
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }
    function exitVid(){
        let vid = document.getElementById(vidElementIdName);
        vid.style.opacity = '0';
        vid.style.pointerEvents = 'none';
        let vidPlayer = document.getElementById(vidElementIdName);
        vidPlayer.pause();
    }
</script>

<main>
    <div class="thumbnail-div" on:click={playVid}>
        <img src="https://i.ytimg.com/vi/{ytVidId}/maxresdefault.jpg" width="320" height="180" alt="{ytVidId} Video Thumbnail" class="thumbnail">
    </div>
    <div class="video" id="{vidElementIdName}" on:click={exitVid}>
        <button on:click={exitVid} class="exit-vid">Exit</button>
        <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/{ytVidId}" 
        title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; 
        encrypted-media; gyroscope; picture-in-picture" allowfullscreen id="vid-player">Loading...</iframe>
    </div>
</main>

<style>
    main{
        width: 335px;
        height: 195px;
    }
    *{
        font-family: 'Roboto', sans-serif;
    }
    iframe{
        /* Align in the middle of the page */
        position: absolute;
        top: calc(50% - 315px/2);
        left: calc(50% - 560px/2);


    }
    .video{
        background-color:rgba(112, 112, 112, 0.514);
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        z-index: 0;
        opacity: 0;
        pointer-events: none;
        transition: opacity 0.5s ease-in-out;
        
    }

    .thumbnail{
        margin: 10px;
        border: 7px solid rgba(56, 56, 56, 0.651);
        border-radius: 10px;
    }
    .thumbnail-div{
        cursor: pointer;
    }
    .exit-vid{
        position: absolute;
        background-color: rgba(255, 255, 255, 0.842);
        color: black;
        border: none;
        border-radius: 5px;
        padding: 5px;
        font-size: 30px;
        cursor: pointer;
        margin: 10px;
    }
</style>