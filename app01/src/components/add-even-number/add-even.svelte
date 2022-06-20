<script>
	let evenNumber2 = [0,2,4,6,8,10];

	const  clickHandler =() => {
		let newNumber2 = evenNumber2[evenNumber2.length-1] + 2;
		//evenNumber2.push(newNumber2) 
		console.log("evenNumber2: " , newNumber2);
        evenNumber2 = [...evenNumber2 , newNumber2]
	}

</script>

<div>
    <button on:click={clickHandler}  class="btn btn-success">Add even num #1</button>
    <p>Result #1: {evenNumber2}</p>
  </div>