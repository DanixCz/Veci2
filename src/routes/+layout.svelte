<script>
    let {children} = $props();
    import Link from './../lib/components/Link.svelte';
    import Button from './../lib/components/Button.svelte';
</script>

<header>
    <a class="logo" href="https://www.arrowheadgamestudios.com/">
        <img class="img" src="/img/Helldivers_2_logo.webp" alt="">
    </a>
    <nav>
        <a class="nav" href="/">Home</a>
        <a class="nav" href="/login">Login</a>
        <a class="nav" href="/register">Sign in</a>
    </nav>
</header>

<main>
    <img class="img2" src="img/HD2_Background2.jpg" alt="">
    {@render children()}
</main>

<style>
@import url('https://fonts.googleapis.com/css2?family=Chakra+Petch:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap');
:global(body){
    margin: 0;
    background-color: rgb(48, 48, 48);
    background-image: url(img/HD2_Background2.jpg);
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
    color: white;
    font-family: "Chakra Petch", sans-serif;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
:global(*){
    font-family: "Chakra Petch", sans-serif;
}
main{
    padding: 0px;
    width: 100%;
    height: 100%;
    margin-top: 155px;
}

header{
    display: flex;
    justify-content: space-between;
    position: fixed;
    width: 100%;
    background-color: rgb(0, 0, 0);
}
nav{
    display: flex;
    align-items: center;
    gap: 50px;
    font-size: 25px;
    padding-right: 78px;
}
.logo{
    margin-top: 25px;
    margin-left: 35px;
    padding-bottom: 25px;
}
.img{
    height: 100px;
}
.img2{
    height: 100%;
    width: 100%;
    position: absolute;
    object-fit: cover;
    z-index: -1;
    top: 0px;
}
.nav{
    transition: 0.5s ease;
    color: rgb(255, 255, 255);
    text-decoration: none;
    font-weight: 600;
    border: 2px solid rgb(0, 0, 0, 0);
    text-shadow: 0px 0px 4px white;
}
.nav:hover{
    color: rgb(255, 233, 0);
    transition: 0.1s;
    border-bottom: 2px solid rgb(255, 233, 0);
    text-shadow: 0px 0px 4px rgb(255, 233, 0);
}

</style>
