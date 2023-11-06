<script>
	import NavbarResponsive from '$lib/navbar_responsive.svelte';
	import HeaderSpacer from '$lib/header_spacer.svelte';
	import Footer from '$lib/footer.svelte';
	import ProductSelector from '$lib/product_selector.svelte';
</script>
<main>
<NavbarResponsive />
<HeaderSpacer />
<div class="flex justify-center align-middle h-16">
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
		<ProductSelector
			product_image='<img alt="" src="./assets/beef_bulgogi_img.png" />'
			product_name='Beef Bulgogi'
			product_price='7.00'
		/>
	</div>
</div>
<Footer />
</main>