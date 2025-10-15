<script lang='ts'>
  let { categories } = $props()
</script>

<aside class="flex flex-col dev">
    <h1>Sidebar</h1>
    {#each categories as category }
        <a class="dev" href="/{category}">{category}</a>
    {/each}
</aside>
