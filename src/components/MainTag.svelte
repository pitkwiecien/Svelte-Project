<script>
    import BgImage from "../components/BgImage.svelte";

    export let imageSrc="";

</script>

<main>
    {#if imageSrc!=""}
        <BgImage src={imageSrc} alt="background"/>
    {/if}
    <slot></slot>
</main>