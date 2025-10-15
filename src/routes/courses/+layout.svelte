<script lang='ts'>
  import SideBar from "$lib/components/SideBar.svelte"

  const categories = ['Item 1', 'Item 2', 'Item 3', 'Item 4', 'Item 5']
  let { children } = $props();
</script>

<div class="flex">
    <div class="ml-4">
        <SideBar {categories} />
    </div>
    <div class="flex-grow flex">
        <div class="w-3/5">
            {@render children?.()}
        </div>
    </div>
</div>
