<script>
	import HeaderSpacer from "$lib/header_spacer.svelte";
	import NavbarResponsive from "$lib/navbar_responsive.svelte";
	import PageTitle from "$lib/page_title.svelte";
	import Footer from "$lib/footer.svelte";
</script>

<main class="">
	<NavbarResponsive />
	<HeaderSpacer />
	<div class="flex justify-center align-middle">
		<PageTitle 
			page_title="About Us"
			page_subtitle="Save a <span class='text-primary-600'>trip</span> to Korea with [SL x FRESHEASY] Meal Kits"
			icon_left=' '
			icon_right='<svg xmlns="http://www.w3.org/2000/svg" class="h6" height="3em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M482.3 192c34.2 0 93.7 29 93.7 64c0 36-59.5 64-93.7 64l-116.6 0L265.2 495.9c-5.7 10-16.3 16.1-27.8 16.1l-56.2 0c-10.6 0-18.3-10.2-15.4-20.4l49-171.6L112 320 68.8 377.6c-3 4-7.8 6.4-12.8 6.4l-42 0c-7.8 0-14-6.3-14-14c0-1.3 .2-2.6 .5-3.9L32 256 .5 145.9c-.4-1.3-.5-2.6-.5-3.9c0-7.8 6.3-14 14-14l42 0c5 0 9.8 2.4 12.8 6.4L112 192l102.9 0-49-171.6C162.9 10.2 170.6 0 181.2 0l56.2 0c11.5 0 22.1 6.2 27.8 16.1L365.7 192l116.6 0z"/></svg>'
		/>
	</div>
	<div class="md:flex md:flex-row-reverse py-12">
		<div class="md:w-1/2 h-max p-6">
			<h4 class="h4 font-semibold text-center pb-4 md:pr-8">Our Passion</h4>
			<p class="text-justify pb-8 md:pr-16">
				We are [SL x FRESHEASY] Meal Kits, your gateway to authentic and delightful Korean cuisine. 
				We are a team of passionate food enthusiats dedicated to bringing the rich and bold flavours 
				of Korea to your home. <br><br>
				Our love for Korean dishes has driven us to create easy-to-cook mealkits that ensure a memorable
				dining experience for you and your loved ones.
			</p>
			<h4 class="h4 font-semibold text-center pb-4 md:pr-8">Our Business</h4>
			<p class="text-justify pb-8 md:pr-16">
				At [SL x FRESHEASY], we take pride in providing you with the highest quality ingredients and recipes
				inspired by traditional Korean cuisine. We've meticulously crafted a selection o meal kits, including
				<a class="text-primary-700 underline" href="beef">Beef Bulgogi</a>,
				<a class="text-primary-700 underline" href="pork">Spicy Pork Bulgogi</a>,
				<a class="text-primary-700 underline" href="chicken">Spicy Chicken Bulgogi</a>, and
				<a class="text-primary-700 underline" href="armystew">Army Stew</a>,
				to cater to your diverse tastes and culinary preferences. <br><br>

				Our commitment is to offer not just a meal, but an adventure in Korean flavours right in your own
				kitchen. Thank you for choosing [SL x FRESHEASY] Meal Kits. We can't wait to embark on this flavorful
				journey with you, one delicious meal at a time.
			</p>
		</div>
		<div class="md:w-1/2 flex flex-row-reverse md:flex-col content-center justify-center">
			<div class="w-1/2 md:w-full flex justify-center py-8">
				<img 
					src="./assets/spicy_pork_bulgogi_img.png" alt=""
					class="-rotate-[10deg] -z-40 pb-8 pr-4 scale-110 md:pb-0 drop-shadow-[-4px_6px_6px_rgba(0,0,0,1)]"
				/>
			</div>
			<div class="w-1/2 md:w-full flex justify-center py-8">
				<img 
					src="./assets/army_stew_img.png" alt=""
					class="rotate-[10deg] -z-40 pb-8 pl-4 scale-110 md:pb-0 drop-shadow-[-4px_6px_6px_rgba(0,0,0,1)]"
				/>
			</div>
		</div>
	</div>
	<Footer />
</main>