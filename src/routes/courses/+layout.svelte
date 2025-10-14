<script lang='ts'>
  import SideBar from "$lib/components/SideBar.svelte"

  const categories = ['Item 1', 'Item 2', 'Item 3', 'Item 4', 'Item 5']
  let { children } = $props();
</script>

<main class="flex">
    <SideBar {categories} />
 {@render children?.()}
</main>
