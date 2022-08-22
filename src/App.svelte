<script>
	import Router from 'svelte-spa-router';
	import About from './routes/About.svelte';
	import Home from './routes/Home.svelte';

	let name;

	let routes = {
		"/" : Home,
		"/about" : About
	}
</script>

<main>
	<Router {routes}/>
</main>

<!--
<script>
import BgImage from "./components/BgImage.svelte";

	import Button from "./components/Button.svelte";
	import FixedBar from "./components/FixedBar.svelte";
import MiddleElement from "./components/MiddleElement.svelte";
import Image from "./components/Image.svelte";
import Link from "./components/Link.svelte";

	export let name;
</script>

<main>
	<BgImage src="/images/background.png" alt="background"/>
	<FixedBar heightPercent=10 bgColor="transparent" fontSize=2 bold={true} generateSafeArea={true}>
		<div slot="left" class="rels">
			<Image src="/images/lightbulb.png" alt="logo" scaling=0.02 marginRight=15/>
			<Image src="/images/text.png" alt="company name" scaling = 0.07 marginRight=20/>
			<Link href="about:blank">O nas</Link>
			<Link href="about:blank">Bezpieczeństwo</Link>
			<Link href="about:blank">Wsparcie</Link>
		</div>
		<div slot="right" class="rels">
			<Button style="secondary">Zaloguj się</Button>
		</div>
	</FixedBar>
	<MiddleElement>
		<div id="middle-text">Połącz pasje!</div>
		<div id="middle-button">
			<Button>Utwórz konto</Button>
		</div>
	</MiddleElement>
	
</main>

<style>
	#middle-text{
		font-size: 7em;
		font-weight: 700;
		color: black;
	}

	#middle-button{
		font-size: 3em;
	}

	.rels {
		display: flex;
		align-items: center;
	}

	main {
		text-align: center;
		padding: 1em;
		max-width: none;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
</style>
-->