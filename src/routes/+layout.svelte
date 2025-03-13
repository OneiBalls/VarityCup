<script lang="ts">
	import '@fontsource-variable/funnel-display';
	import '@fontsource-variable/inter';
	import '../app.css';
	let { children } = $props();
</script>

<header class="navbar shadow-sm">
	<div class="navbar-start">
		<img class="size-10" src="eventlogo.png" alt="Onei's Variety Cup">
	</div>
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