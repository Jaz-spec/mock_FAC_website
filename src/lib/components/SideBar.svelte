<script lang='ts'>
  let { summaries } = $props()
</script>

<aside class="flex flex-col border-t-4 w-full border-b-4 border-yellow-300 mt-5">
    {#each summaries as post, index }
        <a class="text-lg p-1 pl-5 text-left {index < summaries.length - 1 ? 'border-b border-yellow-300' : ''}" href="/courses/{post.slug}">{post.title}</a>
    {/each}
</aside>
