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
	<div class="flex justify-center items-center">
	</div>
	<Footer />
</main>