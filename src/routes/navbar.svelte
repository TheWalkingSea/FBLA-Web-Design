<script type="ts">
    import logo from './lib/images/logo.png';
    import User from './user.svelte'
    const h: string = "64";
    export let userid: Number;

</script>
<nav class="navbar p-2 pr-5">    
    <div class="navbar-brand">
        <a href="/" class="navbar-item">
            <img src={logo} alt="logo" width={128}>
        </a>
        <div class="navbar-burger">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
        </div> 
    </div>
    <div class="navbar-menu columns is-vcentered">
        <div class="navbar-end">
            <a href="/about" class="navbar-item is-active">About</a>
            <a href="/rocket" class="navbar-item">The Rocket</a>
            <a href="/contact" class="navbar-item">Contact</a>
            <a href="/booking" class="navbar-item">Booking</a>
            <a href="/rewards" class="navbar-item">Rewards</a>
            {#if userid}
                <a href="/profile" class="navbar-item"><User {userid}/></a> 
            {:else}
                <button class="button is-primary">Sign In</button>
            {/if}
        </div>
    </div>
</nav>


<style lang="scss">
    .navbar-end {
        gap: 5px;
    }
    .navbar-end a::after {
        transition: width .4s;
    }
    .navbar-end a:hover::after {
        width: 80%;
    }
    .navbar-end a::after {
        content: "";
        position: absolute;
        height: 1.8px;
        width: 0%;
        left: 50%;
        background-color: black;
        bottom: 15%;
        
        
    }
</style>