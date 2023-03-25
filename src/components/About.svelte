<script>
	import Description from './Description.svelte';
	import Felt from './Felt.svelte';
	import Gallery from './Gallery.svelte';
</script>

<div class="container-about">
	<div class="container-title">
		<Felt title="About Us" />
	</div>
	<div class="container-description">
		<div class="content">
			<Felt title="Who We Are" />
			<Description 
				description="We pride ourselves on 
      being the most loved 
      furniture store in the world.
      We've got everything 
      from couches, to beds,
      to dining tables, 
      and much more."
			/>
		</div>
		<div class="image">
      <figure class="content-image">
				<Gallery image="https://i.postimg.cc/J0c2PYJG/Rectangle-2.png" title="image"/>
			</figure>
      <figure class="content-image image-center">
				<Gallery image="https://i.postimg.cc/kgZfFPZT/Rectangle-3.png" title="image"/>
			</figure>
      <figure class="content-image image-up">
				<Gallery image="https://i.postimg.cc/BQngrvfh/Rectangle-4.png" title="image"/>
			</figure>
    </div>
	</div>
</div>

<style>
	.container-about {
		font-family: Arial, Helvetica, sans-serif;
	}
	.container-title {
		text-align: center;
		padding: 2.2rem;
	}
	.container-description {
		display: flex;
		padding: 2rem;
	}
	.content {
		display: flex;
		flex-direction: column;
	}
	.image {
		display: flex;
		align-items: center;
		gap: 1.8rem;
	}
	.content-image {
		align-self: flex-end;
		margin: 0;
	}
	.image-center {
		align-self: flex-end;
		margin-bottom: -0.2rem;
	}
	.image-up {
		align-self: flex-start;
		margin-top: -4rem;
	}
</style>
