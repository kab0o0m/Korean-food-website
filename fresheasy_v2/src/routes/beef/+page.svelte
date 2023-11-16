<svelte:head>
	<title>[SLxFE] - Beef Bulgogi</title>
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
	import ProductCounter from "$lib/product_counter.svelte";
	import ProductSelectorCondensed from "$lib/product_selector_condensed.svelte";
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
			page_subtitle="Our recipes include the finest ingredients, ensuring a <span class='text-primary-600'>restaurant-quality</span> meal.<br>&nbsp;"
			icon_left=''
			icon_right=''
		/>
	</div>
	<div class="flex justify-center flex-col items-center bg-white ">
		<div class="w-full flex lg:flex-row flex-col p-4">
			<div class="w-full flex justify-center">
				<img class="w-[360px] lg:w-[480px] h-[266px] lg:h-[355px] lg:ml-32 mt-8 lg:my-8" src="./assets/beef_bulgogi_img.png"  alt=""/>
			</div>
			<div class="w-full px-12 py-8 lg:px-24 lg:py-16">
				<h3 class="h3 font-semibold text-center lg:text-left">Beef Bulgogi</h3>
				<h4 class="h4 text-center lg:text-left">$8.00</h4>
				<div class="pt-6"><ul class="flex justify-center lg:justify-normal pb-4 space-x-1">
					<li><svg class="fill-primary-500" xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"/></svg></li>
					<li><svg class="fill-primary-500" xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"/></svg></li>
					<li><svg class="fill-primary-500" xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"/></svg></li>
					<li><svg class="fill-primary-500" xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"/></svg></li>
					<li><svg class="fill-primary-500" xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"/></svg></li>
				</ul></div>
				<hr class="bg-gray-500 h-0.5 my-8 w-full lg:w-4/5">
				<div class="flex justify-center lg:justify-normal">
					<div class="lg:flex-none flex-col justify-center">
						<h4 class="h4 font-semibold pb-4 lg:pr-4 lg:pt-1 text-center">Quantity</h4>
						<ProductCounter />
					</div>
				</div>
				<div class="flex justify-center lg:justify-normal py-8">
					<button class="btn bg-primary-500 py-2 px-8 rounded-xl hover:bg-yellow-600">
						<p class="text-white font-semibold pb-1">ADD TO CART</p>
					</button>
				</div>
			</div>
		</div>
		<div class="w-full flex lg:flex-row flex-col p-4">
			<div class="w-full ml-1/2 flex flex-col lg:pl-24">
				<h3 class="h3 lg:text-left text-center font-semibold py-4">Cooking Instructions</h3>
				<ol class="list-decimal ml-8 py-2 mr-4">
					<li>
						<p>Fully defrost all ingredients in the meal kit.</p>
					</li>
					<li>
						<p>Mix the ingredients with the sauce.</p>
					</li>
					<li>
						<p>Add a spoonful of oil to a pan and heat it up over a medium flame for 1 minute.</p>
					</li>
					<li>
						<p>Add the ingredients and stir-fry over medium-to-high heat for 3 minutes, or as desired.</p>
					</li>
					<li>
						<p>Enjoy your beef bulgogi!</p>
					</li>
				</ol>
			</div>
			<div class="w-full">
				<h3 class="h3 lg:text-left text-center font-semibold py-4">Ingredients</h3>
				<ul class="space-y-6">
					<li class="lg:mr-32">
						<div class="flex pt-3">
							<img class="w-24" alt="" src="./assets/beef_bulgogi/beef.png" />
							<p class="text-justify px-4 pt-2">Our meal kit includes the finest cuts of <b>beef</b>, thinly sliced for quick and easy cooking.</p>
						</div>
					</li>
					<li class="lg:mr-32">
						<div class="flex">
							<img class="w-24" alt="" src="./assets/beef_bulgogi/bulgogi_sauce.png" />
							<p class="text-justify px-4 pt-2">Our secret <b>bulgogi sauce</b> recipe guarantees a mouthwatering blend of sweet and savoury.</p>
						</div>
					</li>
					<li class="lg:mr-32">
						<div class="flex">
							<img class="w-24" alt="" src="./assets/beef_bulgogi/vegetable.png" />
							<p class="text-justify px-4 pt-2">We've selected the freshest <b>vegetables and herbs</b> for that authentic touch.</p>
						</div>
					</li>
				</ul>
			</div>
		</div>
		<h2 class="h2 text-center pt-12 font-semibold">View our other meal kits!</h2>
		<div class="flex flex-wrap lg:flex-nowrap justify-center text-center content-center pt-8 pb-32 bg-white w-full">
			<ProductSelectorCondensed
				image_src='./assets/army_stew_img.png'
				product_name='Army Stew'
				product='armystew'
			/>
			<ProductSelectorCondensed
				image_src='./assets/spicy_chicken_bulgogi_img.png'
				product_name='Spicy Chicken Bulgogi'
				product='chicken'
			/>
			<ProductSelectorCondensed
				image_src='./assets/spicy_pork_bulgogi_img.png'
				product_name='Spicy Pork Bulgogi'
				product='pork'
			/>
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