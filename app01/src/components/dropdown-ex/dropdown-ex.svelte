<script>
	let country = 'India' ;

	function changeHandler(event){
		country = event.target.value
	} 
    export let name = "Fantasy";

function changeName(event) {
    const updatedName = event.target.value;
    name = updatedName
}
</script>

<h6>Dropdown Options</h6>

{#if country}
<p>Selection: {country}</p>
{/if}

<select on:input={changeHandler}>
	<option value="Australia">Australia</option>
	<option value="India" selected>India</option>
	<option value="United States">United States</option>
    <option value="Germany">Germany</option>
    <option value="France">France</option>
</select>
<p>Welcome to the {name} Library</p>
<input on:keyup="{changeName}"/>

