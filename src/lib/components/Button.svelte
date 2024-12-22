<script>
	import Button from './Button.svelte';
    let {color, children} = $props();
</script>

<button class="button {color}">
    {@render children()}
</button>

<style>
.button{
    padding: 8px;
    min-height: 50px;
    min-width: 100px;
    text-align: center;
}

.button.blue{
    background-color: rgb(0, 110, 255);
    color: white;
}

.button.green{
    background-color: rgb(1, 121, 11);
    color: white;
}

.button.white{
    background-color: white;
    color: black;
}
</style>