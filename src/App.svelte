<script>
	$: name = "";
	$: numb = "";
	$: email = "";
	const proceed = () => {
		document.getElementById('conten').innerHTML = `Name: ${name}, Email: ${email}, Whatsapp: ${numb}`
	}

</script>

<main class="container">
	<h1>Meeting Schedular</h1>
	<p>In order to book a time slot with me, fill out the details correctly and proceed forward to select the timeslot that works best for you.</p>
	<p><b>Note: You can not book more than two slots per week</b></p>
	<form>
		<input type="text" value={name} name="Name" id="name" placeholder="Full name">
		<input type="text" value={numb} name="Email" id="email" placeholder="Email">
		<input type="text" value={email} name="Number" id="number" placeholder="WhatsApp Number e.g. +923482777095">
		<button on:click={proceed}>Proceed Forward</button>
	</form>
	<div id="conten">
		Name: {name}
		Email: {email}
		Whatsapp: {numb}
	</div>
</main>