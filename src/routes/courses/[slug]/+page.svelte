<script lang="ts">
  let { data }: { data: any } = $props();
</script>

<h1 class="text-4xl text-center mt-10">{data.post.title}</h1>
<div>{@html data.post.content}</div>
