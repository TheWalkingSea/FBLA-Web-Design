<script lang="ts">
    import Dropdown from './dropdown.svelte';
    let drop: Element;
    let dropdown = (e: Event) => {(<Element>e.currentTarget).classList.toggle('is-active')}
    function submit(event: Event) {
        event.preventDefault()
        alert("You submitted!")
    }

</script>

        
<Dropdown name="Desinations">
    <button>Tampa</button>
    <button>Tampsdadasa</button>
    <button>Tampa</button>
    <button>Tampadsads</button>
    <button>Tampa</button>
    <button>Tampa</button>
</Dropdown>



<style lang="scss">
    * {
        background-color: rgba(43,43,43,255);
        color: white;
    }
</style>