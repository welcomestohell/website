<script lang="ts">
	import './layout.css';
	import Favicon from '$lib/assets/favicon.png';
	import Logo from '$lib/assets/logo.png';

	import '@fontsource/titillium-web/200.css';
	import '@fontsource/titillium-web/300.css';
	import '@fontsource/titillium-web/400.css';
	import '@fontsource/titillium-web/600.css';
	import '@fontsource/titillium-web/700.css';
	import '@fontsource/titillium-web/900.css';
	import '@fontsource/titillium-web/200-italic.css';
	import '@fontsource/titillium-web/300-italic.css';
	import '@fontsource/titillium-web/400-italic.css';
	import '@fontsource/titillium-web/600-italic.css';
	import '@fontsource/titillium-web/700-italic.css';

	let { children } = $props();
</script>

<svelte:head>
	<title>Welcome To Hell</title>
	<link rel="icon" href={Favicon} />
	<meta name="title" content="Welcome To Hell" />
	<meta
		name="description"
		content="Welcome To Hell is an experimental tower-obby game with inventive gameplay expanding on true-to-its-roots inspirations, all woven together with a rewarding narrative, set in an incinerated Caelum."
	/>
	<meta
		name="keywords"
		content="wth, wthrblx, wthgame, welcomestohell, welcome to hell, etoh, eternal towers of hell, jukes towers of hell, roblox, tower, tower obby, obby, obbying"
	/>
	<meta name="robots" content="noindex, nofollow" />
	<meta name="language" content="English" />
	<meta name="theme-color" content="#8F5921" /><meta name="twitter:title" content="Welcome To Hell" />
	<meta
		name="twitter:description"
		content="Welcome To Hell is an experimental tower-obby game with inventive gameplay expanding on true-to-its-roots inspirations, all woven together with a rewarding narrative, set in an incinerated Caelum."
	/>
	<meta name="twitter:image" content={Logo} />
</svelte:head>

<main>
	{@render children()}
</main>
