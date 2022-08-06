<script>
    export let src;
    export let alt;
    export let scaling = 1;
    export let marginTop = 0;
    export let marginBottom = 0;
    export let marginLeft = 0;
    export let marginRight = 0;

    let image = new Image();
    image.src = src;
    
    let height;
    let width;
    image.onload = () => {
        height = image.height * scaling;
        width = image.width * scaling;
    }
</script>

<img {height} {width} {src} {alt} style="--margin-top: {marginTop}px; --margin-bottom: {marginBottom}px; --margin-left: {marginLeft}px; --margin-right: {marginRight}px;"/>

<style>
    img {
        margin-top: var(--margin-top);
        margin-bottom: var(--margin-bottom);
        margin-left: var(--margin-left);
        margin-right: var(--margin-right);
    }
</style>