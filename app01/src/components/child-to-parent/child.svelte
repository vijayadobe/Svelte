<script>

    import { createEventDispatcher } from "svelte";

    const dispatch = createEventDispatcher();

    function msgHandler() {
      dispatch("mymessage", {
        text: "The event message has been sent from the child, & received at a higher level."
      });
    }

  </script>
  
  <p>Child</p>
  <button on:click={msgHandler}  class="btn btn-primary">
               Forward this Child Evt (Custom)</button>