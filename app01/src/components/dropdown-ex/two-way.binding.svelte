<script>
	let username = '';
	let username2 = '';
    let policy_accepted = false;
	function inputHandler(event){
		username = event.target.value
	}
</script>




<p>Two way Binding</p>
<input type="text" id="username" placeholder ="Type any username" 
       value={username} on:input={inputHandler}>

<p>User name:  {username}</p>

<input type="text" id="username" placeholder ="Type another Username (bind)" bind:value={username2}>
<p> UserName2 : {username2}</p>
<div>
	<input type=checkbox id="policy_accepted" bind:checked={policy_accepted}>
	I have read and accept the privacy policy.
</div>
<button class="btn  btn-primary" disabled={!policy_accepted}>button</button>
<style>
	input {border:1px solid black; margin-bottom: 1em;}
</style>
