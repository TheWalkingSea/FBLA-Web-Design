<script type="ts">
    import { onMount } from 'svelte';
  import Infocards from './infocards.svelte';
    import Navbar from './navbar.svelte';
    let search: HTMLElement;
    function submit(event: Event) {
        event.preventDefault()
        console.log(event)
    }
</script>
<Navbar userid={0}/>


<<<<<<< Updated upstream
=======
    <div class="is-flex is-flex-direction-column is-flex-grow-1">
        <div class="is-flex-grow-2 content is-justify-content-center" id="JetRocketHook">
            <p>Travel Faster than a<br><strong>Jet.</strong></p>
            <p>Travel in a <strong>Rocket.</strong></p>
        </div>
        <div class="is-flex-grow-1"><Finder/></div>
        
    </div>
>>>>>>> Stashed changes

<div class="columns is-justify-content-space-around">
    <Infocards title={"Rewards"}> 
        <p>

            Rewards program
        </p>
    </Infocards>
    <Infocards title={"Our Mission"}> 
        <p>
            Our Mission
        </p>
    </Infocards>
    <Infocards title={"The Rocket"}> 
        <p>
            The Rocket
        </p>
    </Infocards>
</div>
    
<style>
    
</style>