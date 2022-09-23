<script>
    import MainTag from "../components/MainTag.svelte";
    import StepBlock from "../components/StepBlock.svelte";
    import {aboutElems} from "../../scripts/stores"
    
    aboutElems.update(n => 1)
</script>

<MainTag barBgColor="#fff">
    <StepBlock image="" imageAlt="">
        <div slot="title">
            Pobierz aplikację
        </div>
        <div slot="main">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sed elementum ante. Nunc at facilisis turpis. Donec sed pulvinar nunc. Ut sit amet faucibus enim, id posuere libero. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec at sapien eget nisl consectetur eleifend vel sed neque. Nullam et malesuada enim. Proin cursus enim sed interdum cursus. Pellentesque ornare nisi ut ante dapibus, nec hendrerit nisl feugiat. Quisque efficitur lacus et aliquam semper. Interdum et malesuada fames ac ante ipsum primis in faucibus. Quisque faucibus, arcu a lobortis maximus, lectus nisi dignissim diam, eu elementum nibh enim eget orci. Donec lobortis.
        </div>
    </StepBlock>
    <StepBlock image="" imageAlt="">
        <div slot="title">
            Ustaw preferencje
        </div>
        <div slot="main">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sed elementum ante. Nunc at facilisis turpis. Donec sed pulvinar nunc. Ut sit amet faucibus enim, id posuere libero. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec at sapien eget nisl consectetur eleifend vel sed neque. Nullam et malesuada enim. Proin cursus enim sed interdum cursus. Pellentesque ornare nisi ut ante dapibus, nec hendrerit nisl feugiat. Quisque efficitur lacus et aliquam semper. Interdum et malesuada fames ac ante ipsum primis in faucibus. Quisque faucibus, arcu a lobortis maximus, lectus nisi dignissim diam, eu elementum nibh enim eget orci. Donec lobortis.
        </div>
    </StepBlock>
    <StepBlock image="" imageAlt="">
        <div slot="title">
            Nawiązuj kontakty
        </div>
        <div slot="main">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sed elementum ante. Nunc at facilisis turpis. Donec sed pulvinar nunc. Ut sit amet faucibus enim, id posuere libero. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec at sapien eget nisl consectetur eleifend vel sed neque. Nullam et malesuada enim. Proin cursus enim sed interdum cursus. Pellentesque ornare nisi ut ante dapibus, nec hendrerit nisl feugiat. Quisque efficitur lacus et aliquam semper. Interdum et malesuada fames ac ante ipsum primis in faucibus. Quisque faucibus, arcu a lobortis maximus, lectus nisi dignissim diam, eu elementum nibh enim eget orci. Donec lobortis.
        </div>
    </StepBlock>
    <StepBlock image="" imageAlt="">
        <div slot="title">
            Rozwijaj się!
        </div>
        <div slot="main">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sed elementum ante. Nunc at facilisis turpis. Donec sed pulvinar nunc. Ut sit amet faucibus enim, id posuere libero. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec at sapien eget nisl consectetur eleifend vel sed neque. Nullam et malesuada enim. Proin cursus enim sed interdum cursus. Pellentesque ornare nisi ut ante dapibus, nec hendrerit nisl feugiat. Quisque efficitur lacus et aliquam semper. Interdum et malesuada fames ac ante ipsum primis in faucibus. Quisque faucibus, arcu a lobortis maximus, lectus nisi dignissim diam, eu elementum nibh enim eget orci. Donec lobortis.
        </div>
    </StepBlock>
</MainTag>

<style>
    
</style>