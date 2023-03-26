<script lang="ts">
	let navbar: HTMLElement;
	import { onMount } from 'svelte';

	let bgClass = '';

	function handleScroll() {
		bgClass = scrollY > 10 ? 'bg-scrolled' : '';
	}
	onMount(() => {
		window.addEventListener('scroll', handleScroll);
	});
</script>

<nav class={bgClass + ' ' + 'navbar'} bind:this={navbar}>
	<div class="container-title">
		<h2 class="title">Felt</h2>
	</div>
	<div class="band">
		<a href="/">Home</a>
		<a href="#about">About</a>
		<a href="#gallery">Gallery</a>
		<a href="#form">Contact</a>
	</div>
</nav>

<style>
	.navbar {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		background-color: transparent;
		z-index: 9999;

		display: flex;
		justify-content: space-between;
		align-items: center;
		height: 70px;
		margin-bottom: 3rem;
	}
	.bg-scrolled {
		background-color: rgba(255, 255, 255, 0.9);
		box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
		transition: background 0.5s;
	}
	.container-title {
		margin-left: 10px;
	}

	.title {
		font-size: 2.5rem;
		margin: 0;
		font-weight: bold;
		font-family: Arial, Helvetica, sans-serif;
		color: #eff2f6;
	}
	.bg-scrolled .title {
		color: #000;
	}

	.band {
		display: flex;
		justify-content: space-between;
		align-items: center;
		height: 50px;
		gap: 4.5rem;
		padding: 0 20px;
	}

	.band a {
		color: #eff2f6;
		text-decoration: none;
		font-size: 16px;
		font-weight: bold;
		font-family: Arial, Helvetica, sans-serif;
	}
	.band a:hover {
		color: #00a6eb;
		transform: scale(1.1);
		transition: color 0.2s ease-in-out, transform 0.2s ease-in-out;
	}
	.bg-scrolled a {
		color: #000;
	}
</style>
