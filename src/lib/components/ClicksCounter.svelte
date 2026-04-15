<script>
    let {
        initialCount: count = $bindable(0),
        willIncrement = () => {},
        didIncrement = () => {}
    } = $props()

    let doubled = $derived(count * 2)

    const increment = () => {
        willIncrement(count)
        count++
        didIncrement(count)
    }
</script>

<h3>Clicks Counter</h3>

<!-- per commentare tenere premuto ctrl e premere prima K e poi C -->
<button onclick={increment}> 
clicks:{count}
</button>

<span>doubled is {doubled}</span>