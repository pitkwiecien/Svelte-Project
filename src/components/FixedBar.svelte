<script>
    export let height = 30;
    export let bgColor = 'white';
    export let color = 'black';
    export let generateSafeArea = true;
</script>

<main>
    <div id="bar" style="--bar-height: {height}; --bar-color: {bgColor}; --font-color: {color}">
        <span class="left">
            <slot name="left" class = "left"/>
        </span>
        <span class="right">
            <slot name="right"/>
        </span>
    </div>
    {#if generateSafeArea}
        <div id="safeArea">&shy;</div>
        ABCASA
    {/if}
</main>

<style>
    #bar {
        color: var(--font-color);
        background-color: var(--bar-color);
        height: var(--bar-height);
        position: fixed;
        width: 100%;
        margin: 0px;
        padding: 5px;
    }

    #safeArea {
        /*background-color: greenyellow;*/
        min-height: var(--bar-height);
        width: 100%;
        margin: 0px;
        margin-bottom: 10px;
    }

    .left {
        float: left;
    }

    .right {
        float: right;
    }
</style>