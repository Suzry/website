<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import NavBar from "$lib/components/navBar.svelte";
    import  Footer  from "$lib/components/Footer.svelte";
</script>

<NavBar/>
<ModeWatcher />
<main class="min-h-[calc(100vh-10.5rem)]">
    <slot/>
</main>
<Footer/>