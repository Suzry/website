<script lang="ts">
    export let date: string;
    export let title: string;
    export let company: string;
    import Container from "./Container.svelte";
</script>
<Container>
    <div class="flex flex-col min-w-32">
        <span class="text-primary font-bold">{date}</span>
        <span class="font-bold">{title}</span>
        <span>{company}</span>
    </div> 
    <div>
        <slot/>
    </div>
</Container>