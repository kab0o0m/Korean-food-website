<svelte:head>
	<title>[SLxFE] - Frequently Asked Questions</title>
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
	import QAndA from "$lib/q_and_a.svelte";
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
			page_title="Frequently Asked Questions"
			page_subtitle="<br>&nbsp;"
			icon_left=''
			icon_right=''
		/>
	</div>
	<div class="bg-white flex flex-col justify-center py-8 lg:px-32">
		<ul class="w-full mx-6 pr-16">
			<li>
				<QAndA 
					question="What kind of meal kits do you have?"
					answer="We have 4 different types of meal kits - 
					
								<a class='text-primary-600 underline' href='beef'>Beef Bulgogi</a>,
								<a class='text-primary-600 underline' href='pork'>Spicy Pork Bulgogi</a>,
								<a class='text-primary-600 underline' href='chicken'>Spicy Chicken Bulgogi</a>, and
								<a class='text-primary-600 underline' href='armystew'>Army Stew</a>.

								All our meal kits are influenced by Korean cuisine."
				/>
			</li>
			<li>
				<QAndA 
					question="How will the meal kits be delivered?"
					answer="The meal kits will be delivered frozen in a thermal bag. Please store them in the freezer once received."
				/>
			</li>
			<li>
				<QAndA 
					question="When will the meal kits be delivered?"
					answer="You can select the day of the week and the time range that's the most convenient for you to receive your meal kit delivery at checkout."
				/>
			</li>
			<li>
				<QAndA 
					question="How many servings are in a box?"
					answer="Each box is good for 2 pax. Feel free to add rice, dumplings, or anything you wish to your meal!"
				/>
			</li>
			<li>
				<QAndA 
					question="How long can I store my meal kits?"
					answer="Our meal kits are good for 2 weeks from delivery if stored in the freezer. Once defrosted, please cook and consume the meal kit within 3 days."
				/>
			</li>
			<li>
				<QAndA 
					question="How much is the delivery fee?"
					answer="The delivery is at a flat rate of $6 to any location in Singapore, but delivery is free if you spend more than $50 in one order."
				/>
			</li>
		</ul>

		<h3 class="h3 text-center pt-8 font-semibold mx-6">Still have unanswered questions?</h3>
		<h3 class="h3 text-center pb-8 font-semibold mx-6">Please fill in our contact form and we will get back to you as soon as possible.</h3>
		<div class="flex justify-center pb-8">
			<a href="contact.html" class="w-48 bg-primary-500 hover:bg-primary-600 rounded-xl pb-1">
				<p class="text-white py-2 text-center pb-2 font-bold">CONTACT US</p>
			</a>
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