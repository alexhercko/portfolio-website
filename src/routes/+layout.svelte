<script lang="ts">
    import { resolve } from '$app/paths';
    import { page } from '$app/state';
    import favicon from '$lib/assets/favicon.svg';
    import '../app.css';

    let { children } = $props();
</script>

<svelte:head>
    <link rel="icon" href={favicon} />
</svelte:head>

<nav>
    <a href={resolve('/')} aria-current={page.url.pathname === '/' ? 'page' : undefined}> Home </a>
    <a href={resolve('/about')} aria-current={page.url.pathname === '/about' ? 'page' : undefined}>
        About
    </a>
</nav>

{@render children()}

<style>
    nav {
        display: flex;
        flex-direction: row;
        justify-content: center;
        padding: 0.4rem;
        border-bottom: 1px solid var(--color-text-secondary);
    }

    nav a {
        color: var(--color-text-secondary);
        text-decoration: none;
        margin: 1rem;
        font-weight: 300;
        text-transform: uppercase;
        font-size: 0.9rem;
    }

    nav a[aria-current='page'] {
        color: var(--color-text);
        font-weight: 400;
    }
</style>
