<script type="ts">
    import { onMount } from 'svelte';
    import Navbar from './navbar.svelte';
    import Finder from './findFlight.svelte';
    let search: HTMLElement;
    function submit(event: Event) {
        event.preventDefault()
        console.log(event)
    }
</script>
<section class="is-fullheight is-flex is-flex-direction-column">
    

    <Navbar userid={0}/>


    <div class="is-flex is-flex-direction-column is-flex-grow-1">
        <div class="is-flex-grow-2 content is-justify-content-center" id="JetRocketHook">
            <p>Travel Faster than a<br><strong>Jet.</strong></p>
            <p>Travel in a <strong>Rocket.</strong></p>
        </div>
        <div class="is-flex-grow-1 field is-align-self-center"><Finder/></div>
        
    </div>

</section>

<style type="scss">
    .is-fullheight {
        height: 100vh;
    }
    p {
        font-size: 2em;
    }
    #JetRocketHook {
        padding-left: 4.5em;
        padding-top: 5em;
    }
</style>

