<!-- <script>
    let count = 0;
    $: doubled = count * 2;
  
    const handleClick = () => {   // changed to an arrow fn.
      count += 1;
    }
  </script>
  
  
  
  <button on:click={handleClick}  class="btn btn-primary">
    Clicked {count} {count === 1 ? 'time' : 'times'}
  </button>
  
  <p>{count} doubled is {doubled}</p> -->

  <script>
    let car = 'Mercedes';
    
  $: carMakeSedan = car + ' E350';
  $: carMakeSuv = car + ' G500';
  </script>
  
  <h5>Reactive Approach</h5>
  <p> The {car} you want is a {carMakeSedan}.</p>
  <p> If you would like something more expensive, go for the {carMakeSuv}.</p>
  