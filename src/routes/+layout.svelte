<script lang="ts">
   import "../app.css";
   import Footer from "$lib/components/Footer.svelte";
   import NavBar from "$lib/components/NavBar.svelte";
   import { page } from '$app/stores';

   let { children } = $props();
</script>

<div class="flex flex-col min-h-screen">
    <NavBar/>
    <main class="flex-grow flex {$page.url.pathname.startsWith('/courses') ? 'justify-between' : 'justify-center'}">
        <div class="w-3/5">
            {@render children?.()}
        </div>
    </main>
    <Footer/>
</div>
