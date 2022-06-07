<script>
    export let icon;
    let open = false;
</script>

<li>
    <a href="#" on:click={() => open = !open}>
        {icon}
    </a>
    {#if open}
        <slot />
    {/if}
</li>


<style>
    li {
        width: calc(var(--nav-size) * 0.8);
        display: flex;
        justify-content: center;
        align-items: center;
    }

    a {
        --button-size: calc(var(--nav-size) * 0.5);
        width: var(--button-size);
        height: var(--button-size);
        background-color: #484a4d;
        border-radius: 50%;
        padding: 5px;
        margin: 2px;

        display: flex;
        justify-content: center;
        align-items: center;

        transition: filter 300ms;
    }

    a:hover {
        filter: brightness(120%);
    }
</style>