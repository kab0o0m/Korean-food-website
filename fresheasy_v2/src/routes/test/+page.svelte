<script>
	import NavbarResponsive from '$lib/navbar_responsive.svelte';
	import HeaderSpacer from '$lib/header_spacer.svelte';
	import ProductSelector from '$lib/product_selector.svelte';
	import PageTitle from '$lib/page_title.svelte';
</script>
<main>
	<NavbarResponsive />
	<HeaderSpacer />
<div class="flex justify-center align-middle">
	<PageTitle 
		page_title="This is the title! This is a <span class='text-primary-600'>test</span>!"
		page_subtitle="This is the subtitle!"
	/>
</div>
<div class="container mx-auto flex justify-center items-center">
</div>
</main>

<style>
</style>