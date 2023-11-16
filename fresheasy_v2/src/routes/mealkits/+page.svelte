<svelte:head>
	<title>[SLxFE] - Mealkits</title>
	<!-- Google tag (gtag.js) -->
	<script async src="https://www.googletagmanager.com/gtag/js?id=G-HN5K1CFH54"></script>
	<script>
	window.dataLayer = window.dataLayer || [];
	function gtag(){dataLayer.push(arguments);}
	gtag('js', new Date());
	gtag('config', 'G-HN5K1CFH54');
	</script>
	<!-- Google Tag Manager -->
	<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
	new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
	j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
	'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
	})(window,document,'script','dataLayer','GTM-PG9P7JQQ');</script>
	<!-- End Google Tag Manager -->
	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Noto+Sans:wght@400;600;700&display=swap">
</svelte:head>

<script>
	import HeaderSpacer from "$lib/header_spacer.svelte";
	import NavbarResponsive from "$lib/navbar_responsive.svelte";
	import PageTitle from "$lib/page_title.svelte";
	import Footer from "$lib/footer.svelte";
	import ProductSelector from '$lib/product_selector.svelte';
</script>

<main>
	<!-- Google Tag Manager (noscript) -->
	<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-PG9P7JQQ"
	height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
	<!-- End Google Tag Manager (noscript) -->

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
				product_price='8.00'
				product='beef'
			/>
			<ProductSelector
				image_src='./assets/spicy_chicken_bulgogi_img.png'
				product_name='Spicy Chicken Bulgogi'
				product_price='8.00'
				product='chicken'
			/>
			<ProductSelector
				image_src='./assets/spicy_pork_bulgogi_img.png'
				product_name='Spicy Pork Bulgogi'
				product_price='8.00'
				product='pork'
			/>
			<ProductSelector
				image_src='./assets/army_stew_img.png'
				product_name='Army Stew'
				product_price='8.00'
				product='armystew'
			/>
		</div>
		<div class="flex justify-center pb-16">
			<a href="checkout.html"><div class="w-48 rounded-lg bg-primary-500 hover:bg-primary-600 text-center h-12 pt-3 text-white font-bold">
				CHECKOUT NOW
			</div></a>
		</div>
	</div>
	<Footer />
</main>
<style>
	p, ol, ul, li, a, b {
		font-family: 'Noto Sans', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}

	h1, h2, h3, h4, h5, h6 {
		font-family: 'Poppins' ,'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}
</style>