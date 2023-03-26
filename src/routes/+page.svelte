<script>
	import About from '../components/About.svelte';
	import GalleryUs from '../components/GalleryUs.svelte';
	import Form from '../components/Form.svelte'

	
</script>

<div class="container-image" />
<main class="container-main">
	<About />
	<GalleryUs />
	<Form/>
</main>

<style>
	.container-image {
		background-image: url('https://i.postimg.cc/KjTXQ5xw/Rectangle-13.png');
		background-size: cover;
		height: 100vh;
	}
	.container-main {
		background-color: #eff2f6;
	}
</style>
