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