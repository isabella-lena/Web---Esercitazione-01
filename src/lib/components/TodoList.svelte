<script>
    let todos = $state([
        {title: "Assignment 1", done: false},
        {title: "Assignment 2", done: false},
        {title: "Assignment 3", done: false},
    ])
</script>

<h3>Todos</h3>

<ul>
    {#each todos as todos}
        <li>{todos.title}</li>
    {/each}
</ul>