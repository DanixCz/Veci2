<script>
	import Link from './../lib/components/Link.svelte';
    import Button from './../lib/components/Button.svelte';
</script>

<svelte:head>
    <title>Home</title>
</svelte:head>

<h1>Welcome to SvelteKit</h1>
<a href="/login">login</a>
<a href="/register">register</a>
<Button color="white">Ahoj</Button>
<Button color="green">Ahoj</Button>
<Button color="blue">Ahoj</Button>
<Button>Ahoj</Button>
<Link href="login" color="blue">Login</Link>

