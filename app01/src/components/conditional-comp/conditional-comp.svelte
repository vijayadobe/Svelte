<!-- <style>
    .btn {
        border: none;
        color: white;
        padding: 14px 28px;
        font-size: 16px;
        cursor: pointer;
        background: orange;
        margin-top: 1.2em;
    }
    </style>

    <script>
        let str = 'Please sign in' ;
        let status = "sign-out" ;
        let btnLabel = 'Sign in' ;
        let disabled = false ;
        
        $: if (status === 'sign-in') {
            str = 'Signed in successfully (and now, the btn is disabled).' ;
            btnLabel = 'Sign out' ;
            disabled = true ;
        }

        const loginHandler = () => status = 'sign-in' ; 
        
    </script>

    <div>
        <div>{str}</div>
        <button disabled={disabled} on:click={loginHandler} class="btn">{btnLabel}</button>
    </div>
 
     -->
     <!-- <script>
        let showText = false;

        const  showHandler = () => showText = true
        
   </script>

   <div>
       <button disabled={showText}  class="btn" on:click={showHandler}>Click to show the text</button>

       {#if showText}
        <p>The if block in markup got executed and the btn is disabled.</p>
       {/if}
   </div>
 

   <style>
       .btn {
           border: none;
           color: white;
           padding: 14px 28px;
           font-size: 16px;
           cursor: pointer;
           background:#ff3e99;
           margin-bottom: 1em;
       }
       </style> -->




<script>
	export let status;
	let str ='' ;

	function statusHandler(){ status = true }

	$:if(status){
		str = 'You are authorized for this application.'
	} else {
		str = 'You are not yet authorized for this appl.'
	}




</script>

<div>
    <p>Status: {str}</p>

    {#if !status}
      <button class="btn" on:click={statusHandler}>Authorize</button>
    {/if}
</div>

<style>
	.btn {
    border: none;
    color: white;
    padding: 14px 28px;
    font-size: 16px;
    cursor: pointer;
     background:#ff3f72;
}
</style>
    
   