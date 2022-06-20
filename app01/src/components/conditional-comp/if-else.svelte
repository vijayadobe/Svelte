<script>
    let luggage = { checkedIn: false };
    const count = 7;
    let active = true;
    function toggle() {
      luggage.checkedIn = !luggage.checkedIn;
    }
    setInterval(()=>{active = !active }, 1000)
  </script>
  
  <h5>Use of if expression</h5>
  
  {#if luggage.checkedIn}
    <button on:click={toggle}  class="btn btn-warning">
      Luggage is Checked Out
    </button>
  {/if}
  
  {#if !luggage.checkedIn}
    <button on:click={toggle}   class="btn btn-danger">
      Luggage is Checked In
    </button>
  {/if}
  
  <div><em>Use of if-else block</em></div>
  
  
  {#if count > 10}
      <p>{count} is greater than 10</p>
  {:else if 5 > count}
      <p>{count} is less than 5</p>
  {:else}
      <p>{count} is between 5 and 10</p>
  {/if}

  <button class="btn {active ? 'active' : 'inactive'}">Button</button>
  <style>
    .btn {
      border: none;
      color: white;
      padding: 14px 28px;
      cursor: pointer;
    }

    .active {background-color: darkorange;} 
    .inactive {background-color: darkred;} 
    </style>