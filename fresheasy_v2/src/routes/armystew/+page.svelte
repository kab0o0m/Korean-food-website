<script>
	import HeaderSpacer from "$lib/header_spacer.svelte";
	import NavbarResponsive from "$lib/navbar_responsive.svelte";
	import PageTitle from "$lib/page_title.svelte";
	import Footer from "$lib/footer.svelte";
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
	<div class="flex justify-center flex-col items-center bg-white ">
		<div class="bg-red-500 w-full flex lg:flex-row flex-col p-4">
			<div class="bg-blue-500 w-full flex justify-center">
				<img class="w-4/5 md:w-2/5 lg:w-1/2 lg:ml-32" src="/assets/army_stew_img.png"  alt=""/>
			</div>
			<div class="bg-yellow-500 w-full lg:p-8">
				<h3 class="h3 text-center lg:text-left">Army Stew</h3>
				<h4 class="h4 text-center lg:text-left">$8.00</h4>
				<hr class="bg-gray-700 my-8 w-full lg:w-4/5">
			</div>
		</div>
		<div class="bg-red-500 w-full flex lg:flex-row flex-col p-4">
			<div class="bg-blue-500 w-full">
				Cooking Directions
			</div>
			<div class="bg-yellow-500 w-full">
				Ingredients List
			</div>
		</div>
		<div class="bg-green-500 w-full flex lg:flex-row flex-col justify-center p-4">
			<div class="bg-blue-500 w-full lg:w-1/3">
				Other Product 1
			</div>
			<div class="bg-yellow-500 w-full lg:w-1/3">
				Other Product 2
			</div>
			<div class="bg-blue-500 w-full lg:w-1/3">
				Other Product 3
			</div>
		</div>
	</div>
	<Footer />
</main>