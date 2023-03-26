<script lang="ts">
	import Gallery from './Gallery.svelte';
	import Felt from './Felt.svelte';
</script>

<div class="container-gallery">
	<div class="title-gallery">
		<Felt title="Gallery" />
	</div>
	<div class="image-gallery">
		<Gallery image="https://i.postimg.cc/cLh2wJGw/Rectangle-6.png" title="image" />

		<Gallery image="https://i.postimg.cc/vZYSYdxB/Rectangle-8.png" title="image" />

		<Gallery image="https://i.postimg.cc/d3c4zMKJ/Rectangle-9.png" title="image" />

		<Gallery image="https://i.postimg.cc/8kLyLChc/Rectangle-10.png" title="image" />

		<Gallery image="https://i.postimg.cc/VNLXWGSS/Rectangle-11.png" title="image" />

		<Gallery image="https://i.postimg.cc/4N5BFF2T/Rectangle-7.png" title="image" />
	</div>
</div>

<style>
	.container-gallery {
		font-family: Arial, Helvetica, sans-serif;
	}
	.title-gallery {
		text-align: center;
		padding: 2.2rem;
	}
	.image-gallery {
		display: flex;
		justify-content: space-around;
		flex-wrap: wrap;
		align-items: center;
		gap: 1rem 1rem;
	}
	
</style>
