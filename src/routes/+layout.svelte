<script lang="ts">
   import "../app.css";
   import Footer from "$lib/components/Footer.svelte";
   import NavBar from "$lib/components/NavBar.svelte";
   import { page } from '$app/stores';

   let { children } = $props();
</script>

<div class="flex flex-col min-h-screen">
    <div class="w-11/12 mx-auto flex flex-col flex-grow">
        <NavBar/>
        <main class="flex-grow flex w-full mt-2 {$page.url.pathname.startsWith('/courses') ? 'justify-between' : 'justify-center'}">
            <div class="{$page.url.pathname.startsWith('/courses') ? 'w-9/10' : 'w-3/4'}">
                {@render children?.()}
            </div>
        </main>
    </div>
    <Footer/>
</div>
