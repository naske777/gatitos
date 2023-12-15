<script>

	import './styles.css';
	import HeaderComponent from '$lib/components/header/headerComponent.svelte';
	import FooterComponent from '$lib/components/footer/footerComponent.svelte';
</script>
<HeaderComponent/>

<div class="container mt-5">
	<slot />
</div>

<FooterComponent/>

