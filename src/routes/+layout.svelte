<script lang="ts">
   import "../app.css";
   import Footer from "$lib/components/Footer.svelte";
   import NavBar from "$lib/components/NavBar.svelte";

   let { children } = $props();
</script>

<NavBar/>
<main>
    {@render children?.()}
</main>
<Footer/>
