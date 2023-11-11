<script>
	import HeaderSpacer from "$lib/header_spacer.svelte";
	import NavbarResponsive from "$lib/navbar_responsive.svelte";
	import PageTitle from "$lib/page_title.svelte";
	import Footer from "$lib/footer.svelte";
	import OrderList from "$lib/order_list.svelte";

	let selected = "creditcard";

	const tomorrow = new Date();
	tomorrow.setDate(tomorrow.getDate() + 1);

	const nextMonth = new Date(); // Create a new Date object for next month
	nextMonth.setDate(tomorrow.getDate() + 30);

	const year = tomorrow.getFullYear();
	const month = String(tomorrow.getMonth() + 1).padStart(2, '0'); // Months are zero-based
	const day = String(tomorrow.getDate()).padStart(2, '0');

	const yearNext = nextMonth.getFullYear();
	const monthNext = String(nextMonth.getMonth() + 1).padStart(2, '0'); // Months are zero-based
	const dayNext = String(nextMonth.getDate()).padStart(2, '0');

	const tomorrowFormatted = `${year}-${month}-${day}`;
	const nextMonthFormatted = `${yearNext}-${monthNext}-${dayNext}`;

	const onPaymentChange = () => {
		selected = event.currentTarget.value;
	}

	const changeToCard = () => { selected = "creditcard"; }
	const changeToPayPal = () => { selected = "paypal"; }
	const changeToPayLah = () => { selected = "paylah"; }
</script>

<main>
	<NavbarResponsive />
	<HeaderSpacer />
	<div class="flex justify-center align-middle">
		<PageTitle 
			page_title="Checkout"
			page_subtitle="Enjoy <span class='text-primary-600'>free shipping</span> for orders above $50"
			icon_left=''
			icon_right='<svg xmlns="http://www.w3.org/2000/svg" class="h6" height="3em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M64 64C28.7 64 0 92.7 0 128v64c0 8.8 7.4 15.7 15.7 18.6C34.5 217.1 48 235 48 256s-13.5 38.9-32.3 45.4C7.4 304.3 0 311.2 0 320v64c0 35.3 28.7 64 64 64H512c35.3 0 64-28.7 64-64V320c0-8.8-7.4-15.7-15.7-18.6C541.5 294.9 528 277 528 256s13.5-38.9 32.3-45.4c8.3-2.9 15.7-9.8 15.7-18.6V128c0-35.3-28.7-64-64-64H64zm64 112l0 160c0 8.8 7.2 16 16 16H432c8.8 0 16-7.2 16-16V176c0-8.8-7.2-16-16-16H144c-8.8 0-16 7.2-16 16zM96 160c0-17.7 14.3-32 32-32H448c17.7 0 32 14.3 32 32V352c0 17.7-14.3 32-32 32H128c-17.7 0-32-14.3-32-32V160z"/></svg>'
		/>
	</div>
	<div class="flex lg:flex-row flex-col bg-white select-none">
		<div class="lg:w-3/5">
			<h3 class="h3 text-center pt-8 pb-4 font-semibold">Order</h3>
			<OrderList />
		</div>
		<div class="lg:w-2/5 lg:py-16 lg:pl-4 lg:pr-16 lg:px-0 px-4">
			<form class="bg-white">
				<label for="contact" class="font-bold">
					Contact Information
				</label>
				<input class="w-full mt-3 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="contact" name placeholder="Full name">
				<div class="w-full flex py-4">
					<input class="w-1/2 mr-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" name placeholder="E-mail">
					<input class="w-1/2 ml-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" name placeholder="Phone">
				</div>
				<label for="contact" class="font-bold">
					Delivery Address
				</label>
				<input class="w-full mt-3 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="contact" name placeholder="Address Line 1">
				<input class="w-full mt-3 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="contact" name placeholder="Address Line 2">
				<div class="w-full flex py-4">
					<input class="w-1/2 mr-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" name placeholder="Unit No.">
					<input class="w-1/2 ml-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" name placeholder="Postal Code">
				</div>
				<div class="flex pb-4">
					<input type="checkbox" id="vehicle1" name="billingaddr" value="same" class="mt-1 rounded-md mr-2">
					<label for="billingaddr" class="text-gray-700">Billing address same as shipping</label><br>
				</div>
				<label for="date" class="font-bold">
					Delivery Date and Time
				</label>
				<input type="date" id="date" class="my-2 border-gray-300 rounded-xl text-gray-700 focus:outline-none" min="{tomorrowFormatted}" max="{nextMonthFormatted}" />
				<ul class="py-2 px-3">
					<li><div class="flex pt-1">
						<input type="radio" name="time" id="9-12" class="mt-1 mr-2" selected />
						<label for="9-12">9am-12pm</label>
					</div></li>
					<li><div class="flex pt-1">
						<input type="radio" name="time" id="12-3" class="mt-1 mr-2"/>
						<label for="12-3">12pm-3pm</label>
					</div></li>
					<li><div class="flex pt-1">
						<input type="radio" name="time" id="3-6" class="mt-1 mr-2"/>
						<label for="3-6">3pm-6pm</label>
					</div></li>
					<li><div class="flex pt-1">
						<input type="radio" name="time" id="6-9" class="mt-1 mr-2"/>
						<label for="6-9">6pm-9pm</label>
					</div></li>
				</ul>
				<label for="paymentmethod" class="font-bold mb-2">
					Payment Method
				</label>
				<div class="select-none px-3 border {selected === 'creditcard' ? 'border-gray-700' : 'border-gray-300'} rounded-lg flex my-2 py-1">
						<input type="radio" name="paymentmethod" value="creditcard" id="creditcard" class="mt-1 mr-2" checked on:change={onPaymentChange}/>
						<label for="creditcard">Credit Card</label>
				</div>
				{#if selected=='creditcard'}
					<div class="px-8 pb-4">
						<input class="w-full mt-3 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="contact" name placeholder="Card number">
						<div class="w-full flex pt-4 pb-2">
							<input class="w-1/4 mr-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" type="month" placeholder="Expiration (MM/YY)">
							<input class="w-1/4 ml-2 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" name placeholder="CVV">
						</div>
						<input class="w-full mt-3 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="contact" name placeholder="Name on card">
						<div class="flex pt-4">
							<input type="checkbox" id="billingaddr" name="billingaddr" value="same" class="mt-1 rounded-md mr-2">
							<label for="billingaddr" class="text-gray-700">Remember me</label><br>
						</div>
					</div>
				{/if}
				<div class="select-none px-3 border {selected === 'paypal' ? 'border-gray-700' : 'border-gray-300'} rounded-lg flex my-2 py-1">
						<input type="radio" name="paymentmethod" value="paypal" id="paypal" class="mt-1 mr-2" on:change={onPaymentChange} />
						<label for="paypal">PayPal</label>
				</div>
				{#if selected=='paypal'}
					<p class="text-gray-500 text-center text-md px-8">After clicking 'Checkout Now', you will be redirected to an external site to proceed with your payment.</p>
				{/if}
				<div class="select-none px-3 border {selected === 'paylah' ? 'border-gray-700' : 'border-gray-300'} rounded-lg flex my-2 py-1">
						<input type="radio" name="paymentmethod" value="paylah" id="paylah" class="mt-1 mr-2" on:change={onPaymentChange} />
						<label for="paylah">PayLah/PayNow</label>
				</div>
				{#if selected=='paylah'}
					<p class="text-gray-500 text-center text-md px-8">After clicking 'Checkout Now', you will be redirected to an external site to proceed with your payment.</p>
				{/if}
				<label for="promocode" class="font-bold">
					Promo Code
				</label>
				<input class="w-1/4 mt-3 appearance-none border border-gray-300 rounded-xl text-gray-700 leading-tight focus:outline-none" id="promocode" name placeholder="">
			</form>
			<div class="bg-primary-500 rounded-xl mx-8 my-8 cursor-pointer hover:bg-primary-700">
				<p class="text-white text-center py-2 px-8 font-bold text-xl">Checkout Now</p>
			</div>
		</div>
	</div>
	<Footer />
</main>