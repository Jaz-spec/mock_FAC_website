<script lang="ts">
  import CoursesNavBar from "$lib/components/CoursesNavBar.svelte";
  import SideBar from "$lib/components/SideBar.svelte"
  import type { Snippet } from 'svelte';

  let { children, data }: { children: Snippet, data: any } = $props();
</script>

<div class="flex justify-between mt-2 w-full">
    <div class="w-2/6 flex-shrink-0">
        <SideBar summaries={data.summaries} />
    </div>
    <div class="flex justify-end">
        <div class="w-11/12">
            {@render children?.()}
        </div>
    </div>
</div>
