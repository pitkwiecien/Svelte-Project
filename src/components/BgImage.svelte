<script>
    export let src;
    export let alt;

    let height = window.outerHeight;
    let width = window.outerWidth;
</script>

<div id="imgbox">
    <img {height} {width} {src} {alt}>
</div>

<style>
    *{
        z-index: -1;
        margin: 0;
        padding: 0;
    }
    
    #imgbox {
        display: grid;
        height: 100%;
    }
        
    img {
        position: absolute;
        top: 0px;
        left: 0px;
        right: 0px;
        margin: 0px;
        padding: 0px;
        max-width: 100%;
        max-height: 100vh;
        margin: auto;
    } 
</style>