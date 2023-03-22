<script>
	import Description from './Description.svelte';
	import Felt from './Felt.svelte';
	import Gallery from './Gallery.svelte';
</script>

<div>
	<div>
		<Felt title="About Us" />
	</div>
	<div>
		<div>
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
		<div>
      <Gallery image="https://i.postimg.cc/J0c2PYJG/Rectangle-2.png" title="image"/>
      <Gallery image="https://i.postimg.cc/kgZfFPZT/Rectangle-3.png" title="image"/>
      <Gallery image="https://i.postimg.cc/BQngrvfh/Rectangle-4.png" title="image"/>
    </div>
	</div>
</div>

<style></style>
