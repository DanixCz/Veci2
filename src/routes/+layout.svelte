<script>
    let {children} = $props();
</script>

<header>
    <nav>
        <a href="/">HOME</a>
        <a href="/login">login</a>
        <a href="/register">register</a>
    </nav>
</header>

<main>
    {@render children()}
</main>

<style>
:global(body){
    margin: 0;
}

main{
    padding: 21px;
}

nav{
    background-color: blue;
    padding: 24px;
}
a{
    color: white;
}
</style>