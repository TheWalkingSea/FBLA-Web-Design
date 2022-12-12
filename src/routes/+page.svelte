<script type="ts">
    import { onMount } from 'svelte';
    import Navbar from './navbar.svelte';
    let search: HTMLElement;
    function submit(event: Event) {
        event.preventDefault()
        console.log(event)
    }
</script>
<Navbar userid={0}/>


<div class="is-flex is-flex-direction-column">
    <div class="is-flex-grow-2 content is-justify-content-center">
        <p>Travel Faster than a<br>Jet.</p>
        <p>Travel in a Rocket.</p>
    </div>
    <form class="is-flex-grow-1" on:submit>
        <div class="field is-grouped is-spaced-evenly is-justify-content-center">
            <div class="control">
                <input name="destination" type="text" class="input" placeholder="Destination">
            </div>
            <div class="control">
                <input name="depart" type="text" class="input" placeholder="Departure">
            </div>
            <div class="control">
                <input name="date" type="text" class="input" placeholder="Date">
            </div>
            <button class="button" type="submit">lorem</button>
        </div>
    </form>
</div>
<style>
    
</style>