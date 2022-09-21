<script>
    import Image from "./Image.svelte";

    export let number;
    export let image;
    export let imageAlt;

    let left = number % 2 == 1
    let stPosition
    if(left){
        stPosition = "left: -45px;"
    } else {
        stPosition = "right: -45px;"
    }

    let lineReversed = left ? "" : "flex-direction: row-reverse;";


</script>

<div id="line" style="{lineReversed}">
    <div id="stepBody">
        <div id="title">
            <div id="numberImage" style="{stPosition}">
                <Image src="/images/circle_{number}.png" alt={number} scaling=0.5/>
            </div>
            <slot name="title"/>
        </div>
        <div id="main">
            <slot name="main"/>
        </div>
    </div>
    <div id="colon">
        *colon*
    </div>
    <div id="img">
        *img*
    </div>
</div>


<style>
    #line {
        margin-left: 10%;
        margin-right: 10%;
        margin-top: 70px;
        display: flex;
    }

    #colon{
        text-align: center;
        position: relative;
        top: 70px;
        margin: 0px;
        width: 10%;
    }

    #img{
        text-align: center;
        position: relative;
        top: 70px;
        width: 40%;
    }

    #stepBody{
        position: relative;
        margin: 0px;
        top: 70px;
        width: 50%;
    }

    #numberImage {
        display: inline-block;
        position: absolute;
        top: -45px;
        z-index: -100;
    }

    #title {
        font-weight: 800;
        font-size: 2em;
        text-decoration: underline;
        text-decoration-color: red;
        text-decoration-thickness: 6px;
        text-underline-offset: 10px;
        margin-bottom: 10px;
        display: inline-block;
        position: relative;
    }

    #main {
        position: relative;
        top: 0px;
        font-size: 1em;
        left: 0px;
    }

</style>