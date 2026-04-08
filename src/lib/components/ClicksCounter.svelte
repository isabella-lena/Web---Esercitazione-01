<script>
    import { on } from "svelte/events";
    let {initialCount} = $props()
    let doubled = $derived(initialCount * 2)
</script>

<h3>Clicks Counter</h3>

<!-- per commentare tenere premuto ctrl e premere prima K e poi C -->
<button onclick={() => initialCount++}> 
clicks:{initialCount}
</button>

<span>doubled is {doubled}</span>