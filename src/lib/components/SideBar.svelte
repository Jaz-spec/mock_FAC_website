<script lang='ts'>
  let { categories } = $props()
</script>

<aside class="flex flex-col">
    <h1>Sidebar</h1>
    {#each categories as category }
        <a href="/{category}">{category}</a>
    {/each}
</aside>
