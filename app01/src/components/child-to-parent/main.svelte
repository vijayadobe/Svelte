<script>
	import Parent from './parent.svelte';


	function handleMessage(event) {
        console.log("in main container...", event);
		alert("main comp: " + event.detail.text);
       
	}
function navigationHandler() {
    alert('jkjsd')
}
</script>


<h6> G_child to G_parent Comms (use of custom msg).</h6>
<p>Main Container</p>
<Parent on:mymessage={handleMessage}/>
<!-- prvent default -->
<a href="http://google.com/" on:click|preventDefault={navigationHandler}>Go to Google</a>