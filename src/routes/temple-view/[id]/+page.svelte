<script>
     
    import { onMount } from 'svelte';
  
    let popVisible = false;
   
    
    function showPop() {
      popVisible = true;
      
      setTimeout(() => {
        popVisible = false;
      }, 2000); // Hide the pop after 2 seconds
    }
  
    // Function to hide the pop on page load
    function hidePop() {
      popVisible = false;
      
      
    }
  
    // Hide the pop on page load
    onMount(() => {
      hidePop();
    });
  </script>
  




<div class="uniqueId">
    <div class="poster">
        <img src="../tofi-banner2.jpg" alt="banner"/>
    </div>
   

    <div class="Icones">
       
       
        <button on:click={showPop}>
        {#if popVisible}
            <img src="../custom_visited.svg" alt="Visited" />
          {:else}
            <img src="../custom_visited_filled.svg" alt="Not Visited" />
          {/if}
          
       
        </button>
        {#if popVisible}
          
          <div class="pop">Pop-up message!</div>
        {/if}
          
        <img src="../custom_favorite.svg" alt="nitLiked"/>
    </div>
</div>
<style>
    .poster,img{
        width:100%;
    }
    .Icones{
        display: flex;
    justify-content: right;
    padding: 20px;
    }
    .Icones img{
        height:30px;
        width:30px;
    }
    
  button{
    border:none;
    background-color: transparent;
  }
</style>