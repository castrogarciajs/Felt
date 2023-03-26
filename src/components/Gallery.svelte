<script lang="ts">
	export let image: string;
	export let title: string;
</script>

<img class="image" src={image} alt={title} />

<style>
	img {
		transition: transform 0.5s;
	}

	img:hover {
		transform: scale(0.9);
	}
</style>
