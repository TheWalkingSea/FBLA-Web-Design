<script lang="ts">
    export let name: String;
    let drop: Element;
</script>

<button class="button" type="button" on:click={() => drop.classList.toggle("active")}>{name}</button>
<div class="expandedDrop" bind:this={drop}>
    <slot/>
</div>


<style lang="scss">
    .active {
        visibility: visible;
    }
    .expandedDrop {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 5px;
        background-color: white;
        padding: 1em;
        visibility: hidden;
    }
    .expandedDrop :global(*) {
        color: rgb(60, 77, 162);
        background-color: white;
        border: none;
        transition: color, .5s;
        font-size: 1.2em;
    }
    .expandedDrop :global(*):hover {
        color: black;
    }
</style>