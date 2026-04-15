<script>
    import{ website } from "$lib/state.svelte.js"
</script>

<h3>{website.title}</h3>

<input type="text" bind:value={website.title}>