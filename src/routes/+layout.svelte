<script>
	import Header from './Header.svelte';
	import First from "./first.svelte";
	import About from './about.svelte';
	import Tech from './tech.svelte';
	import Social from './social.svelte';
	import Footer from './footer.svelte';
	import './styles.css';
    import Project from './project.svelte';
</script>

<div class="app">
	<Header />
	<First />
	<About />
	<Tech />
	<Project />
	<Social />
	<Footer />
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		align-items: center;
		
	}
</style>