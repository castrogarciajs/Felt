<script>
	import Felt from './Felt.svelte';
	import Gallery from './Gallery.svelte';
</script>

<div class="container-form">
	<div class="title-form">
		<Felt title="Contact Us" />
	</div>
	<div class="container-content">
		<div class="container-form--active">
			<form action="" class="form">
				<label for="name-user"> Name </label>
				<input class="input-name" type="text" id="name-user" />
				<label for="email-user"> Email </label>
				<input class="email-user" type="email" id="email-user" />
				<label for="description-user"> Message </label>
				<textarea class="text-area" id="description-user" cols="30" rows="15" />
			</form>
		</div>
		<div class="container-image-form">
			<!--image-->
			<Gallery image="https://i.postimg.cc/CKxmxHgg/Rectangle-17.png" title="image" />
		</div>
	</div>
</div>

<style>
	.container-form {
		font-family: Arial, Helvetica, sans-serif;
	}
	.title-form {
		text-align: center;
		padding: 2.2rem;
	}
	.container-content {
		display: flex;
		justify-content: space-evenly;
		align-items: center;
	}
	.form {
		display: flex;
		gap: 1rem;
		flex-direction: column;
		
	}
  input, textarea {
    background-color: #BAC4C4;
    outline: none;
    border-radius: 5px;
    border: none;
  }
  input {
    width: 500px;
    height: 40px;
  }
  label {
    font-weight: bold;
    font-size: 1.5rem;
  }
</style>
