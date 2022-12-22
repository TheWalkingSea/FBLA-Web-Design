<script lang="ts">
    import Dropdown from './dropdown.svelte';
    function submit(event: Event) {
        event.preventDefault()
        alert("You submitted!")
    }
    const destinations = ["Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", "Tampa", "New York", ]

</script>

<div class="is-flex is-justify-content-space-around">
    <div class="dropdowns columns is-3">
        <div class="column">
            <Dropdown name="Destinations">
                {#each destinations as dest}
                    <button>{dest}</button>
                {/each}
            </Dropdown>
        </div>
        <div class="column">
            <Dropdown name="Departure">
                {#each destinations as dest}
                    <button>{dest}</button>
                {/each}
            </Dropdown>
        </div>
        <div class="column">
            <Dropdown name="Destinations">
                {#each destinations as dest}
                    <button>{dest}</button>
                {/each}
            </Dropdown>
        </div>
    </div>
    <div class="submit">
        <button class="button">Find Flight</button>
    </div>
</div>



<style lang="scss">
    .dropdowns {
        overflow: visible;
    }
    * {
        background-color: rgba(43,43,43,255);
        color: white;
    }

</style>