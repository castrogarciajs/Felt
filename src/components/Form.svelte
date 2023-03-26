<script>
	import Felt from './Felt.svelte';
	import Gallery from './Gallery.svelte';
</script>

<section class="container-form" id="form">
	<div class="title-form">
		<Felt title="Contact Us" />
	</div>
	<div class="container-content">
		<div class="container-form--active">
      <h2>Drop us a Message </h2>
			<form action="" class="form">
				<label for="name-user"> Name </label>
				<input class="input-name" type="text" id="name-user" placeholder="name"/>
				<label for="email-user"> Email </label>
				<input class="email-user" type="email" id="email-user" placeholder="email"/>
				<label for="description-user"> Message </label>
				<textarea class="text-area" id="description-user" cols="30" rows="15" placeholder="Description" />
        <button type="submit">Submit</button>
			</form>
		</div>
		<div class="container-image-form">
			<!--image-->
			<Gallery image="https://i.postimg.cc/CKxmxHgg/Rectangle-17.png" title="image" />
		</div>
	</div>
</section>

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
  h2 {
    font-size: 2rem
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
  button {
    width: 200px;
    height: 40px;
    background-color: #000;
    color: #fff;
    border: none;
    border-radius: 20px;
    cursor: pointer;
		font-weight: bold;
  }
</style>
