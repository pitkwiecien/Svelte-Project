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