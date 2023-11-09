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
			page_title="About Us"
			page_subtitle="Save a <span class='text-primary-600'>trip</span> to Korea with [SL x FRESHEASY] Meal Kits"
			icon_left=' '
			icon_right='<svg xmlns="http://www.w3.org/2000/svg" class="h6" height="3em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M482.3 192c34.2 0 93.7 29 93.7 64c0 36-59.5 64-93.7 64l-116.6 0L265.2 495.9c-5.7 10-16.3 16.1-27.8 16.1l-56.2 0c-10.6 0-18.3-10.2-15.4-20.4l49-171.6L112 320 68.8 377.6c-3 4-7.8 6.4-12.8 6.4l-42 0c-7.8 0-14-6.3-14-14c0-1.3 .2-2.6 .5-3.9L32 256 .5 145.9c-.4-1.3-.5-2.6-.5-3.9c0-7.8 6.3-14 14-14l42 0c5 0 9.8 2.4 12.8 6.4L112 192l102.9 0-49-171.6C162.9 10.2 170.6 0 181.2 0l56.2 0c11.5 0 22.1 6.2 27.8 16.1L365.7 192l116.6 0z"/></svg>'
		/>
	</div>
	<div class="md:flex md:flex-row-reverse py-12">
		<div class="md:w-1/2 h-max p-6">
			<h4 class="h4 font-semibold text-center pb-4 md:pr-8">Our Passion</h4>
			<p class="text-justify pb-8 md:pr-16">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea veritatis assumenda minima quae harum nulla sunt, laboriosam earum amet pariatur. Alias totam, impedit exercitationem fugit qui at cum, voluptates sit mollitia voluptas officia. Distinctio commodi, praesentium a quod cumque laboriosam dolores ullam aperiam excepturi maiores magnam neque dignissimos nemo pariatur.</p>
			<h4 class="h4 font-semibold text-center pb-4 md:pr-8">Our Business</h4>
			<p class="text-justify pb-8 md:pr-16">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit assumenda numquam officia cumque rem provident doloremque sequi ad tempore, omnis ipsa. Rerum laboriosam tempora laudantium quisquam libero possimus quibusdam reiciendis illum doloremque nesciunt obcaecati amet, iure provident exercitationem aut error numquam assumenda saepe, et non voluptates consectetur modi! Quod exercitationem eos et aperiam esse voluptatem corporis, laborum soluta obcaecati tempora, porro molestias repellat atque officiis. Perspiciatis beatae blanditiis amet accusantium error, ea commodi repellat nam quo reprehenderit molestias enim dolore architecto, rerum facilis fugiat quos aperiam esse, maxime pariatur minus! Enim, minima consequuntur dolore a omnis sequi quas earum voluptates?</p>
		</div>
		<div class="md:w-1/2 flex flex-row-reverse md:flex-col content-center justify-center">
			<div class="w-1/2 md:w-full flex justify-center py-8">
				<img 
					src="./assets/spicy_pork_bulgogi_img.png" alt=""
					class="-rotate-[10deg] -z-50 pb-8 pr-4 scale-110 md:pb-0 drop-shadow-[-4px_6px_6px_rgba(0,0,0,1)]"
				/>
			</div>
			<div class="w-1/2 md:w-full flex justify-center py-8">
				<img 
					src="./assets/army_stew_img.png" alt=""
					class="rotate-[10deg] -z-50 pb-8 pl-4 scale-110 md:pb-0 drop-shadow-[-4px_6px_6px_rgba(0,0,0,1)]"
				/>
			</div>
		</div>
	</div>
	<Footer />
</main>