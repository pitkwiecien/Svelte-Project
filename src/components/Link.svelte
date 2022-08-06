<script>
    export let href;
</script>

<a {href}><slot/></a>

<style>
    a {
        text-decoration: none;
    }

    a:link{
        color: black;
    }
    
    a:hover {
        transform: scale(0.98);
        color: rgb(100, 100, 100);
    }

    a:active{
        color: rgb(150,150,150);
    }

    * {
        margin: 10px;
    }
</style>