<script>
    // @ts-nocheck

    import Button from "$lib/components/ui/button/button.svelte";
    import { page } from "$app/stores";
    import { text } from "@sveltejs/kit";
    import ThemeSwitch from "./themeSwitch.svelte";
    import * as Sheet from "$lib/components/ui/sheet";

    const links = [
        {
            text: "About Me",
            href: "/",
        },
        {
            text: "Resume",
            href: "/resume",
        },
        {
            text: "Projects",
            href: "/projects",
        },
        {
            text: "Contact",
            href: "/contact",
        },
    ];
    let isSheetOpen = false;
</script>

<div
    class="shadow-xl  bg-secondary text-secondary-foreground py-8 px-6"
>
    <nav class="max-w-screen-2xl flex items-center justify-between mx-auto">
        <div class="flex items-center gap-2">
            <div class="bg-primary w-5 h-5 me-4" />
            <div class="flex items-end gap-1">
                <span class="font-bold text-3xl">Mohammed</span>
                <span class="text-xl">/ Developer</span>
            </div>
        </div>

        <div class="flex ">
            <ThemeSwitch/>
            <!-- large -->
            <div class="uppercase hidden lg:flex">
                {#each links as link}
                    <Button
                        class=" {$page.url.pathname == link.href &&
                            'text-primary'}"
                        href={link.href}
                        variant="link"
                        >{link.text}
                    </Button>
                {/each}
            </div>

            <!-- small -->
            <Sheet.Root bind:open={isSheetOpen}>
                <Sheet.Trigger class="flex lg:hidden">
                    <Button class size="icon" variant="ghost">
                        <svg
                        class="w-6 h-auto"
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 512 512"
                            ><path
                                fill="none"
                                stroke="currentColor"
                                stroke-linecap="round"
                                stroke-miterlimit="10"
                                stroke-width="48"
                                d="M88 152h336M88 256h336M88 360h336"
                            /></svg
                        >
                    </Button>
                </Sheet.Trigger>
                <Sheet.Content class="flex flex-col items-center justify-center">
                    {#each links as link}
                    <Button
                        class="text-xl  {$page.url.pathname == link.href &&
                            'text-primary'}"
                        href={link.href}
                        variant="link"
                        on:click={()=> isSheetOpen = false}
                        >{link.text}
                    </Button>
                {/each}
                </Sheet.Content>
            </Sheet.Root>

        </div>
    </nav>
</div>
