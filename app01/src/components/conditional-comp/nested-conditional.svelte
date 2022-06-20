<script>
    let age = 10;
    let status = "";
  
  
    $: if (age > 19) {
      status = "Adult";
    } else if (age > 10 && age < 19) {
      status = "Teenager";
    } else {
      status = "Child";
    }
    
  </script>
  
  <div>
    <div>Use of JS logic:</div>
    <p>Age is {age} and the status is {status}</p>
  </div>
  
  <aside>
    <div>Alt. way (html): </div>
  
    {#if age > 19}
      <div>The age is {age} and so, an Adult.</div>
    {:else if age > 10 && age < 19}
      <div>The age is {age} and so, a Teenager.</div>
    {:else}
      <div>The age is {age} and so, a Child.</div>
    {/if}
  </aside>
  