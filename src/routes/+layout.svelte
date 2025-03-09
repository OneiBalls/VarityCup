<script lang="ts">
	import '@fontsource-variable/funnel-display'
	import '../app.css';
	let { children } = $props();
</script>

<header class="flex items-center justify-between m-4 ">
	<p class="font-display font-bold text-2xl">Pretend this is banner rawr</p>
    <nav>
		<a href="/">Info</a>
		<a href="/standings">Standings</a>
		<a href="/games">Games</a>
		<a href="/teams">Teams</a>
	</nav>
</header>

<!-- Replace this with a UI theme -->
<main class="border-black border-y-2">
	{@render children()}
</main>

<footer>
	aaaaaaaaaaaaaaaa
</footer>