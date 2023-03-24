<script>
import Felt from './Felt.svelte'
</script>

<div>
  <div>
  <Felt title="Contact Us"/>
  </div>
  <div>
  <form action="">
    <label for="name-user">
      Name
      <input type="text" id="name-user" />
    </label>
    <label for="email-user">
      Email
      <input type="email" id="email-user" />
    </label>
    <label for="description-user">
      Message
      <textarea id="description-user" cols="30" rows="10" />
    </label>
  </form>
  </div>
</div>
