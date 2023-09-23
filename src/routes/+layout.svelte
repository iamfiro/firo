<script>
	import Header from './Header.svelte';
	import First from "./first.svelte";
	import About from './about.svelte';
	import Tech from './tech.svelte';
	import Footer from './footer.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />
	<First />
	<About />
	<Tech />
	<Footer />
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		align-items: center;
		
	}
</style>