<script>
    import { on } from "svelte/events";
    let {initialCount: count = $bindable()} = $props()
    let doubled = $derived(count * 2)
</script>

<h3>Clicks Counter</h3>

<!-- per commentare tenere premuto ctrl e premere prima K e poi C -->
<button onclick={() => count++}> 
clicks:{count}
</button>

<span>doubled is {doubled}</span>