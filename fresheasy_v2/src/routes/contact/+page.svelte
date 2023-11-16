<svelte:head>
	<title>[SLxFE] - Contact Us</title>
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
</script>

<main class="bg-white">
	<!-- Google Tag Manager (noscript) -->
	<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-PG9P7JQQ"
	height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
	<!-- End Google Tag Manager (noscript) -->

	<NavbarResponsive />
	<HeaderSpacer />
	<div class="flex justify-center align-middle">
		<PageTitle 
			page_title="Contact Us"
			page_subtitle="We value your questions, feedback, and inquiries. Please don't hesitate to reach out to us through any of the following channels. We're here to assist you in any way we can."
			icon_left='<svg xmlns="http://www.w3.org/2000/svg" height="3em" viewBox="0 0 512 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M256 48C141.1 48 48 141.1 48 256v40c0 13.3-10.7 24-24 24s-24-10.7-24-24V256C0 114.6 114.6 0 256 0S512 114.6 512 256V400.1c0 48.6-39.4 88-88.1 88L313.6 488c-8.3 14.3-23.8 24-41.6 24H240c-26.5 0-48-21.5-48-48s21.5-48 48-48h32c17.8 0 33.3 9.7 41.6 24l110.4 .1c22.1 0 40-17.9 40-40V256c0-114.9-93.1-208-208-208zM144 208h16c17.7 0 32 14.3 32 32V352c0 17.7-14.3 32-32 32H144c-35.3 0-64-28.7-64-64V272c0-35.3 28.7-64 64-64zm224 0c35.3 0 64 28.7 64 64v48c0 35.3-28.7 64-64 64H352c-17.7 0-32-14.3-32-32V240c0-17.7 14.3-32 32-32h16z"/></svg>'
			icon_right=''
		/>
	</div>
	<h2 class="h2 bg-white text-center font-semibold py-16 w-full">Contact Us Directly</h2>
	<div class="flex flex-col lg:flex-row justify-center items-center pb-16">
		<div class="flex flex-col justify-center lg:w-1/2 w-full px-8 lg:block lg:pl-16 xl:pl-32">
			<div class="flex justify-center lg:justify-normal">
				<h4 class="h4 font-semibold pt-1">SUBMIT A TICKET</h4>
				<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-10 pl-4">
					<path stroke-linecap="round" stroke-linejoin="round" d="M16.5 6v.75m0 3v.75m0 3v.75m0 3V18m-9-5.25h5.25M7.5 15h3M3.375 5.25c-.621 0-1.125.504-1.125 1.125v3.026a2.999 2.999 0 010 5.198v3.026c0 .621.504 1.125 1.125 1.125h17.25c.621 0 1.125-.504 1.125-1.125v-3.026a2.999 2.999 0 010-5.198V6.375c0-.621-.504-1.125-1.125-1.125H3.375z" />
				</svg>
			</div>
			<input class="w-full mt-3 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="contact" name placeholder="Full name">
			<div class="w-full flex py-4">
				<input class="w-1/2 mr-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" name placeholder="E-mail">
				<input class="w-1/2 ml-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" name placeholder="Phone">
			</div>
			<input class="w-full my-1 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="contact" name placeholder="Full name">
			<textarea
				class="w-full my-4 mr-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none"
				id="message"
				rows="5"
				placeholder="Message"
			/>

			<div class="flex pt-2 pb-6">
				<input type="checkbox" id="terms" name="billingaddr" value="same" class="mt-1 rounded-md mr-2">
				<label for="terms" class="text-gray-700 pt-1 text-xs">I have read and agree to SL Fresheasy's <a class="underline" href="privacy.html">Privacy Policy</a></label><br>
			</div>
			<div class="flex justify-center pb-4">
				<button class="btn bg-primary-500 w-32 rounded-xl p-2 text-center hover:bg-primary-700 cursor-pointer select-none">
					Send Message
				</button>
			</div>
		</div>
		<div class="bg-white lg:w-1/2 w-full flex justify-center lg:block">
			<table class="ml-8 my-8 mr-8 lg:mr-0">
			<tr class="">
				<td class="py-4 flex justify-center">
				<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-8 pr-4">
					<path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 002.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 01-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 00-1.091-.852H4.5A2.25 2.25 0 002.25 4.5v2.25z" />
				</svg>
				</td>
				<td>
				<a href="tel:+6566841261" class=" text-xl lg:text-2xl underline">+65 6684 1261</a>
				</td>
			</tr>
			<tr>
				<td class="py-4 flex justify-center">
				<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-8 pr-4">
					<path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75" />
				</svg>
				</td>
				<td>
				<a href="mailto:contact@slfoods.com" class=" text-xl lg:text-2xl underline">contact@slfoods.com</a>
				</td>
			</tr>
			<tr>
				<td class="py-4 flex justify-center">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-8 pr-4" viewBox="0 0 320 512">
					<!-- Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
					<path d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z" />
				</svg>
				</td>
				<td>
				<a href="https://www.facebook.com/slfoods.sg/.html" class=" text-xl lg:text-2xl underline">https://www.facebook.com/slfoods.sg/</a>
				</td>
			</tr>
			<tr>
				<td class="py-4 flex justify-center">
					<svg xmlns="http://www.w3.org/2000/svg" class="h-8 pr-4" viewBox="0 0 448 512">
						<!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
						<path d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z"/>
					</svg>
				</td>
				<td>
				<a href="https://www.instagram.com/sl_sharelife.html" class=" text-xl lg:text-2xl underline">https://www.instagram.com/sl_sharelife</a>
				</td>
			</tr>
			</table>

		</div>
	</div>
	<Footer />
</main>
<style>
	p, ol, ul, li, a, b, input, label {
		font-family: 'Noto Sans', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}

	h1, h2, h3, h4, h5, h6 {
		font-family: 'Poppins' ,'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}
</style>