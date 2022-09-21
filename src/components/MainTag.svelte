<script>
    import BgImage from "../components/BgImage.svelte";
    import FilledFixedBar from "../components/FilledFixedBar.svelte";

    export let imageSrc = "";
    export let fixedBar = true;
    export let barBgColor = 'transparent';
    export let barGenerateSafeArea = true;
</script>

<main>
    {#if imageSrc!=""}
        <BgImage src={imageSrc} alt="background"/>
    {/if}
    {#if fixedBar}
        <FilledFixedBar bgColor = {barBgColor} generateSafeArea = {barGenerateSafeArea}/>
    {/if}
    <slot></slot>
</main>