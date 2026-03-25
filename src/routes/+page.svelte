<script>
    import { on } from "svelte/events";

console.log("hello world")
let count = $state(0)
let doubled = $derived(count * 2)
</script>
<h1>Welcome to SveteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>


<button onclick={() => count++}>
clicks:{count}
</button>

<span></span>
<style> 
h1 {
	color:deepskyblue;

}



</style>