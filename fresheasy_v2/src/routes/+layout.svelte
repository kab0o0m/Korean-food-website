<script>
	import './../app.postcss';
	import { AppShell } from '@skeletonlabs/skeleton';
	
	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
	let title = "Sharelife x Fresheasy";
</script>

<head>
	<title>{title}</title>
</head>

<!-- App Shell -->
<AppShell>
	<!-- Page Route Content -->
	<slot />
</AppShell>
