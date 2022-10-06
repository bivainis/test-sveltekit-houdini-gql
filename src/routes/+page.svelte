<script>
  // TODO: what should be the type of data?
  export let data;

  $: ({ GetAllFilms } = data);
</script>

<h1>Star wars films</h1>

{#each $GetAllFilms.data.allFilms.films as { title }, i}
  <li>
    {title}
  </li>
{/each}
