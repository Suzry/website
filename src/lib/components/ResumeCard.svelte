<script lang="ts">
    export let date: string;
    export let title: string;
    export let company: string;
    import Container from "./Container.svelte";
</script>
<div class="rounded-xl bg-secondary p-8 shadow-xl flex flex-col sm:flex-row items-center gap-16">
    <div class="flex flex-col min-w-32">
        <span class="text-primary font-bold">{date}</span>
        <span class="font-bold">{title}</span>
        <span>{company}</span>
    </div> 
    <div>
        <slot/>
    </div>
</div>