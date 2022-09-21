<script>
    export let heightPercent = -1;
    export let heightPixels = 30;
    export let bgColor = 'transparent';
    export let color = 'black';
    export let generateSafeArea = true;
    export let fontSize = 1;
    export let bold = false;

    let fontWeight = bold ? 700 : 400;
    let amount = (heightPercent == -1 ? heightPixels : 0.01 * heightPercent * window.outerHeight);
    let barString = " height: " + amount + "px;";
    let safeAreaString = " padding-bottom: " + amount + "px;";

    function addStyle(styleString) {
        const style = document.createElement('style');
        style.textContent = styleString;
        console.log(style);
        document.head.append(style);
    }

    /*
    let leftHeightString  = "div[slot=\"left\"]{" + barString + "}";
    let rightHeightString  = "div[slot=\"right\"]{" + barString + "}";

    addStyle(leftHeightString);
    addStyle(rightHeightString);
    */
</script>

<div id="bar" style="{barString} --bar-color: {bgColor}; --font-color: {color}; --font-size: {fontSize}em; --font-weight: {fontWeight};">
    <div id="left">
        <slot name="left"/>
    </div>
    <div id="right">
        <slot name="right"/>
    </div>
</div>
{#if generateSafeArea}
    <div id="safeArea" style="{safeAreaString}"></div>
{/if}

<style>
    #bar {
        align-items: center;
        color: var(--font-color);
        background-color: var(--bar-color);
        position: fixed;
        width: 100%;
        margin: 0px;
        padding: 5px;
        font-size: var(--font-size);
        font-weight: var(--font-weight);
        z-index: 10000000;
    }

    #safeArea {
        height: 0px;
        width: 100%;
        margin: 0px;
    }

    #left {
        align-items: center;
        position: absolute;
        left: 16px;
        top: 50%;
        transform: translateY(-50%);
        float: left;
    }

    #right {
        vertical-align: middle;
        align-items: center;
        position: absolute;
        right: 16px;
        top: 50%;
        transform: translateY(-50%);
        float: right;
        text-align: right;
    }

    

</style>