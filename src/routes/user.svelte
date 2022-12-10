<script lang="ts">
    import { onMount } from "svelte";
    export let userid: Number;

</script>
<figure class="image is-48x48">
    <img src={`/src/routes/lib/images/user${userid}.png`} alt="userProfile" class="is-rounded overrideHeight">
</figure>



<style lang="scss">
    .overrideHeight {
        max-height: fit-content;
    }
</style>

