<script lang="ts">
    export let title: string;
    export let subtitle: string;
    export let imageSrc: string;
    import Button from "./ui/button/button.svelte";
</script>

<div class="rounded-xl bg-secondary shadow-xl flex flex-col sm:flex-row gap-4">
    <div class=" flex flex-col gap-16 pt-8">
        <div class="flex flex-col min-w-32 border-s-8 border-primary ps-8">
            <span class="font-bold text-primary text-xl">{title}</span>
            <span>{subtitle}</span>
        </div>
        <div class="ps-8 pb-8">
            <slot />
        </div>
    </div>
    <img
        src={imageSrc}
        alt="صورة للمشروع"
        class="rounded-xl w-auto sm:w-64 object-cover"
        />
</div>
