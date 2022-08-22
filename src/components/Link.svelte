<script>
    import {push, pop, replace} from 'svelte-spa-router';

    export let href;
    export let method = "push";

    function anchor(){
        switch(method){
            case "push":
                push(href);
                break;
            case "pop":
                pop(href);
                break;
            case "replace":
                replace(href);
                break;
            default:
                console.log("INVALID METHOD FOR LINK TO: " + href);
                break;
        }
    }
</script>

<span on:click={anchor}><slot/></span>

<style>
    span {
        text-decoration: none;
    }

    span:link{
        color: black;
    }
    
    span:hover {
        transform: scale(0.98);
        color: rgb(100, 100, 100);
    }

    span:active{
        color: rgb(150,150,150);
    }

    * {
        margin: 10px;
    }
</style>