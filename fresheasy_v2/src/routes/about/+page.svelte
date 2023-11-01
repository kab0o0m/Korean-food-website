<script>
	import HeaderSpacer from "$lib/header_spacer.svelte";
	import NavbarResponsive from "$lib/navbar_responsive.svelte";

</script>

<main>
	<NavbarResponsive />
	<HeaderSpacer />
	<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-10 text-center flex flex-col items-center">
		<h2 class="h2">This is the about page!</h2>
		<!-- Animated Logo -->
		<div class="flex justify-center space-x-2">
		</div>
		<div class="space-y-2">
			<p>Try editing the following:</p>
			<p><code class="code bg-lime-700 text-white">/src/routes/about/+page.svelte</code></p>
		</div>
	</div>
</div>
</main>