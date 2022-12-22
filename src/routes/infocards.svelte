<script type="ts">
    export let title: String;
</script>
<div class="is-flex is-flex-direction-column is-align-items-center">
    <h1 class="content has-text-centered p-6">{title}</h1>

    <div class="card">
        <div class="card-image">
            <figure class="image is-4by3">
                <img src={`/src/routes/lib/images/${title.toLowerCase()}.png`} alt="card decribing content">
            </figure>
        </div>
        <div class="card-content">
            <slot/>
        </div>
    </div>
</div>


<style>
    .card {
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: .3s;
        border-radius: 10px;
        padding: 1em;
        width: 25vw;
    }
    .card:hover{
        box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
    }
</style>