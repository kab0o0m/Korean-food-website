<script>
	import HeaderSpacer from "$lib/header_spacer.svelte";
	import NavbarResponsive from "$lib/navbar_responsive.svelte";
	import PageTitle from "$lib/page_title.svelte";
	import Footer from "$lib/footer.svelte";
	import ProductSelector from '$lib/product_selector.svelte';
</script>

<main>
	<NavbarResponsive />
	<HeaderSpacer />
	<div class="flex justify-center align-middle">
		<PageTitle 
			page_title="Meal Kits"
			page_subtitle="Our recipes include the finest ingredients, ensuring a <span class='text-primary-600'>restaurant-quality</span> meal."
			icon_left=''
			icon_right=''
		/>
	</div>
	<div class="mx-auto flex flex-col justify-center items-center bg-white">
		<h2 class="h2 text-center pt-8 font-bold">Our Meal Kits</h2>
		<div class="flex flex-wrap lg:flex-nowrap justify-center text-center content-center py-8 bg-white w-full">
			<ProductSelector
				image_src='./assets/beef_bulgogi_img.png'
				product_name='Beef Bulgogi'
				product_price='6.00'
				product='beef'
			/>
			<ProductSelector
				image_src='./assets/spicy_chicken_bulgogi_img.png'
				product_name='Spicy Chicken Bulgogi'
				product_price='6.00'
				product='chicken'
			/>
			<ProductSelector
				image_src='./assets/spicy_pork_bulgogi_img.png'
				product_name='Spicy Pork Bulgogi'
				product_price='6.00'
				product='pork'
			/>
			<ProductSelector
				image_src='./assets/army_stew_img.png'
				product_name='Army Stew'
				product_price='6.00'
				product='armystew'
			/>
		</div>
		<div class="flex justify-center pb-16">
			<a href="checkout"><div class="w-48 rounded-lg bg-primary-500 hover:bg-primary-600 text-center h-12 pt-3 text-white font-bold">
				CHECKOUT NOW
			</div></a>
		</div>
	</div>
	<Footer />
</main>