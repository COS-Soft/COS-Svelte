<svelte:head>
    <title>COS Hard To Find Software Page</title>
</svelte:head>

<script>
    import NavigationBar from "../components/NavigationBar.svelte";
    import SoftwareDownload from "../components/SoftwareDownload.svelte";
</script>

<main>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&amp;display=swap" rel="stylesheet">
    <NavigationBar pageName="Hard To Find Software" />
    <SoftwareDownload filePath="../files/htfs/microsoftSrcLeakCollection.torrent" fileName="microsoftSrcLeakCollection"/>
    <SoftwareDownload filePath="../files/htfs/SAMSUNG_LEAK.torrent" fileName="Samsung Galaxy Source Code Leak"/>
</main>

<style>
</style>