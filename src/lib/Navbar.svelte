<nav>
    <ul>
        <slot />
    </ul>
</nav>

<style>
    nav {
        height: var(--nav-size);
        background-color: var(--bg);
        padding: 0  1rem;
    }

    ul {
        max-width: 100%;
        height: 100%;
        display: flex;
        justify-content: flex-end;
    }
</style>