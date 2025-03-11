<script lang="ts">
	import '@fontsource-variable/funnel-display';
	import '@fontsource-variable/inter';
	import '../app.css';
	let { children } = $props();
</script>

<header class="navbar shadow-sm">
	<p class="navbar-start font-display text-2xl font-bold">Onei's Variety Cup</p>
	<nav class="navbar-end">
		<ul class="menu menu-horizontal">
			<li>
				<a href="/">Home</a>
			</li>
			<li>
				<a href="/event">Event</a>
			</li>
		</ul>
	</nav>
</header>

{@render children()}

<!-- TODO: use Dock for mobile -->
<footer>aaaaaaaaaaaaaaaa</footer>
