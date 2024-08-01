<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import NavBar from "$lib/components/navBar.svelte";
</script>

<NavBar/>
<ModeWatcher />
<slot></slot>
