<script>
    export let bgColor = "transparent";
</script>

<div id="middleElement" style="--background-color: {bgColor}">
    <slot></slot>
</div>

<style>
    #middleElement {
        background-color: var(--background-color);
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
        margin-bottom: 0px;
    }
</style> 