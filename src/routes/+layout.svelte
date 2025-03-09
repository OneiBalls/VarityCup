<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<div class='h-screen w-screen bg-gray-400'>
    <div class='text-3xl border border-red-400 border-dotted'>
		<p>Pretend this is banner rawr</p>
        <!-- Erm we put this as static? -->
    </div>
    <nav>
		<a href="/">Info</a>
		<a href="/standings">Standings</a>
		<a href="/games">Games</a>
		<a href="/teams">Teams</a>
	</nav>
    <div class='main'>
		{@render children()}
	</div> 
</div>