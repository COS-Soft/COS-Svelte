<script>
    export let filePath = "";
    export let fileName = "";
</script>

<main>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&amp;display=swap" rel="stylesheet">
    <div>
        <h3>{fileName}</h3>
        <a href="{filePath}" download><button>Download</button></a>
    </div>
</main>

<style>
     *{
        font-family: 'Roboto', sans-serif;
     }
     button{
        background-color: rgb(218, 218, 218);
        margin: 5px;
        border: none;
        width: 200px;
        transition: all 0.3s ease-in-out;
        border-radius: 10px;
        font-size: 20px;
    }
    button:hover{
        background-color: rgb(56, 56, 56);
        color: white;
    }
    div{
        margin: 20px;
        max-width: 1200px;
    }
</style>