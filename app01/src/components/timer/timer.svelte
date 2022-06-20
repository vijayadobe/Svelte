<!-- <script>
    let seconds = 0;
    setInterval(() => seconds += 1, 1000);
  </script>
  
  <h5>A Stateful Component</h5>
  
  <div> Time elapsed in secs: {seconds}  </div> -->

  <script>
	let counter = 0;
    let counterSquare = 0;
	$: {
    counterSquare = counter * counter;

    if (counter % 2 === 0) {
      console.log("Counter is even with value: ", counter);
    } else {
      console.log("Counter is odd with value: ", counter);
    }

  }
	
	function clickHandler(){
		counter += 1
	}
</script>



<div>
    <button on:click={clickHandler}  class="btn btn-primary">Click</button>

    <div>Square of {counter} is {counterSquare}</div>
    <div>Clicked:  {counter} times</div>
    
</div>