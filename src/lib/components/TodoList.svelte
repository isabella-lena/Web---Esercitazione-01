<script>
    let todos = $state([
        {title: "Assignment 1", done: false},
        {title: "Assignment 2", done: true},
        {title: "Assignment 3", done: false},
    ])

    let groceries = $state([
        {title: "Apple", done: false},
        {title: "Bread", done: true},
        {title: "Salmon", done: false},
    ])
</script>

{#snippet todoItem(todo)}
    <li>
        <input type="checkbox" bind:checked={todo.done}>
        {todo.title}
    </li>
{/snippet}

<h3>Todos</h3>

<ul>
    {#each todos as todo}
    {@render todoItem(todo)} 
    {/each}
</ul>

<h3>Groceries</h3>
<ul>
    {#each groceries as grocery}
    {@render todoItem(grocery)} 
    {/each}
</ul>