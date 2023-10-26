<script>
	import './../app.postcss';
	import { AppShell, AppBar } from '@skeletonlabs/skeleton';

	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
	let title = "Sharelife x Fresheasy"
</script>

<head>
	<title>{title}</title>
</head>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar>
			<svelte:fragment slot="lead">
				<strong class="text-xl uppercase">SL x Fresheasy</strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<a
					href="/"
					rel="noreferrer"
				>
					Home
				</a>
				<a
					href="/about"
					rel="noreferrer"
				>
					About
				</a>
				<a
					href="/mealkits"
					rel="noreferrer"
				>
					Meal Kits
				</a>
				<a
					href="/faq"
					rel="noreferrer"
				>
					FAQ
				</a>
				<a
					href="/contact"
					rel="noreferrer"
				>
					Contact Us
				</a>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
