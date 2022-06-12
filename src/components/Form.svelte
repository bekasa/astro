<script>
function submitForm(e) {
    const formData = new FormData(e.target);

    const data = {};
    for (let field of formData) {
      const [key, value] = field;
      data[key] = value;
    }
    console.log(data)
  }


</script>

<form on:submit|preventDefault={submitForm} >
<div class="invisible"><input name="bot-field" /></div>
	<div class="m-2 p-4">
	<div><label for="name">Name<span class="text-red-700">*</span></label></div>
	<input type="text" name="name" id="name" required minlength="4" maxlength="100">
	</div>
	<div class="m-2 p-4">
	<div><label for="email">Email<span class="text-red-700">*</span></label></div>
	<input type="email" name="email" id="email" required >
	</div>
	<div class="m-2 p-4">
	<div><label for="message">Message<span class="text-red-700">*</span></label></div>
	<textarea name="message" cols="30" rows="6" minlength="4" required></textarea>
	</div>
	<div>
	<button class="rounded bg-blue-700 px-4 py-2 m-2 text-white"type="submit">Send</button>
	</div>
</form>