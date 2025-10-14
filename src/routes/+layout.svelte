<script lang="ts">
   import "../app.css";
   import Footer from "$lib/components/footer.svelte";
   import NavBar from "$lib/components/navBar.svelte";
   import SideBar from "$lib/components/sideBar.svelte";

   let { children } = $props();
</script>

<NavBar/>
<main class="flex justify-around ">
    <SideBar/>
    {@render children?.()}
</main>
<Footer/>
