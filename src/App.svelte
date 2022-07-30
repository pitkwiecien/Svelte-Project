<script>
	import Button from "./components/Button.svelte";
	import FixedBar from "./components/FixedBar.svelte";

	export let name;
</script>

<main>
	<FixedBar>
		<span slot="left">
			ABC
		</span>
		<span slot="right">
			DEF
		</span>
	</FixedBar>
	<Button>Utwórz konto</Button>
	<Button style="secondary">Zaloguj się</Button>
	<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
	dadad
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>