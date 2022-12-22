<script>
  import "../app.scss";
</script>

<slot />

<style lang="scss">
  :global(*){
    font-family: Arial, Helvetica, sans-serif;
    color: white;
    background-color: black;
    // font-size: 1.2em;
    }
    :global(i) {
        color: white;
    }
</style>

