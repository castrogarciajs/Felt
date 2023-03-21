<nav class="navbar">
	<div class="container-title">
		<h2 class="title">Felt</h2>
	</div>
	<div class="band">
		<a href="/">Home</a>
		<a href="/about">About</a>
		<a href="products">Products</a>
		<a href="gallery">Gallery</a>
		<a href="/contact">Contact</a>
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
</style>
