<script>
    let {children} = $props();
    import Link from './../lib/components/Link.svelte';
    import Button from './../lib/components/Button.svelte';
</script>

<header>
    <nav>
        <Link href="/" color="white">Home</Link>
        <Link href="/login" color="white">Login</Link>
        <Link href="/registr" color="white">Sign in</Link>
    </nav>
</header>

<main>
    {@render children()}
</main>

<style>
:global(body){
    margin: 0;
    background-color: rgb(48, 48, 48);
}

main{
    padding: 21px;
}

nav{
    background-color: rgb(255, 165, 44);
    padding: 24px;
    gap: 50px;
}
a{
    color: white;
}
</style>