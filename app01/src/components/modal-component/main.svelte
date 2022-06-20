<script>
    import ModalComponent from './modal.svelte' ;

    let showModal = false ;

    </script>


    <h6> Modal Window</h6>
    <button class="btn btn-primary" on:click={()=>showModal = true}>Open Modal</button>

    {#if showModal}
        <ModalComponent
          headerText="Svelte Modal"
          bodyText="This Modal is a child component. An evt from the child informs the parent to close it."
          on:closeEvent={()=>{showModal = false}} >
          
        </ModalComponent>

    {/if}
