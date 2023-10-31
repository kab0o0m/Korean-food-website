<script>
	import Hero from '$lib/hero.svelte'
	import NavbarResponsive from '$lib/navbar_responsive.svelte';
</script>

<main>
<NavbarResponsive />
<div class="flex justify-center align-middle h-screen">
	<Hero />
</div>
<div class="container mx-auto flex justify-center items-center">
	<div class="space-y-10 text-center flex flex-col items-center">
		<h2 class="h2">This is the home page!</h2>
		<div class="flex justify-center space-x-2">
		</div>
		<div class="space-y-2">
			<p>Try editing the following:</p>
			<p><code class="code">/src/routes/+layout.svelte</code></p>
			<p><code class="code">/src/routes/+page.svelte</code></p>
		</div>
	</div>
</div>
</main>