<script>
    import { slide, fly } from 'svelte/transition'
</script>

<div transition:slide>
    <a href="#" transition:fly= "{{ x: 200, duration: 2000 }}">
        hi
        <span class="icon-right"></span>
    </a>
</div>

<style>
    div {
        position: absolute;
        top: 58px;
        width: 300px;
        transform: translateX(-45%);
        background-color: var(--bg);
        border: var(--border);
        border-radius: var(--border-radius);
        padding: 1rem;
        overflow: hidden;
    }

    a {
        height: 50px;
        display: flex;
        align-items: center;
        border-radius: var(--border-radius);
        transition: background-color var(--speed);
        padding: 0.5rem;
    }

    a:hover {
        background-color: #525357;
    }

    .icon-right {
        margin-left: auto;
    }
</style>