<script>
    import Button from "../components/Button.svelte";
    import MainTag from "../components/MainTag.svelte";
    import FilledFixedBar from "../components/FilledFixedBar.svelte";
    import MiddleElement from "../components/MiddleElement.svelte";
</script>
    
<MainTag imageSrc="/images/background.png">
    <FilledFixedBar/>
    <MiddleElement>
        <div id="middle-text">Połącz pasje!</div>
        <div id="middle-button">
            <Button>Utwórz konto</Button>
        </div>
    </MiddleElement>
</MainTag>
    
<style>
    #middle-text{
        font-size: 7em;
        font-weight: 700;
        color: black;
    }
    
    #middle-button{
        font-size: 3em;
    }
</style>