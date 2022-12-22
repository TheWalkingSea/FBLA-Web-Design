<script lang="ts">
    export let name: String;
    $: active = false;
</script>

<div class="parent">
    <button class:active type="button" on:mousedown={() => active = !active}>
        <div class="icon-text">
            <span class="icon">
                <i class="fa-solid fa-location-dot"></i>
            </span>
            <span class="name">{name}</span>
            <span class="icon right">
                <i class="fa-solid fa-caret-down"></i>
            </span>
        </div>
    </button>
    <div class="expandedDrop" class:active>
        <slot/>
    </div>
</div>

<style lang="scss">
    $dropdown: rgb(86, 86, 86);
    $buttontext: white;
    button {
        font-size: 1.2em;
    }
</style>