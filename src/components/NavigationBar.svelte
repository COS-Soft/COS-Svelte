<script>
    export let pageName = "";
</script>

<main>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&amp;display=swap" rel="stylesheet">
    <link rel="icon" type="image/x-icon" href="./favicon.png">
    <meta name="google-site-verification" content="M2jFTTmjjIYIOfBUsOnBPRXDm4orSXpHDBnkKpNxXJc">


        <nav>
            <a href="/"><img src="/favicon.png" alt="7-Times Logo"></a>
            <h1>COS {pageName} Page</h1>
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/videos">Videos</a></li>
                <li><a href="/hardtofindsoftware">Hard To Find Software</a></li>
                <li><a href="/about">About</a></li>
            </ul>
        </nav>

    
</main>

<style>
    /* Roboto Font*/
    *{
        font-family: 'Roboto', sans-serif;
    }
    main{
        margin: 0;
    }
    nav{
        background-color: rgb(56, 56, 56);
        display: flex;
        align-items: center;
        padding: 1rem;
    }
    nav img{
        border-radius: 10px;
        width: 100px;
        height: 100px;
        margin-right: 30px;
    }
    nav h1{
        color: white;
        font-size: 2rem;
        font-weight: bold;
        text-align: center;
        background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
	    background-size: 400% 400%;
	    animation: gradient 10s ease infinite;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }
    nav ul{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-left: auto;
    }
    nav ul li{
        list-style: none;
        margin: 0 1rem;
    }
    nav ul li a{
        color: white;
        text-decoration: none;
        font-size: 1.2rem;
        font-weight: bold;
        transition: all 0.3s ease-in-out;
    }
    nav ul li a:hover{
        /* make the text color gradient on hover */
        background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
	    background-size: 400% 400%;
	    animation: gradient 10s ease infinite;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;

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
    @media screen and (max-width: 600px){
        nav{
            flex-direction: column;
            align-items: center;
        }
        nav img{
            width: 50px;
            height: 50px;
        }
        nav h1{
            font-size: 1.5rem;
        }
        nav ul{
            flex-direction: column;
            align-items: center;
        }
        nav ul li{
            margin: 0.5rem 0;
        }
        nav ul li a{
            font-size: 1rem;
        }
    }

   

    
</style>