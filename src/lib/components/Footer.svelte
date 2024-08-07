<script>
    import SocialMedia from "./SocialMedia.svelte";
</script>
<footer class=" bg-secondary text-secondary-foreground py-2 px-6">
    <div class="max-w-screen-2xl flex md:flex-row flex-row-reverse  items-center justify-between mx-auto ">
        <span class="self-end md:self-center">
            ©{(new Date()).getFullYear()} by Mohammed
        </span>
        <div class="flex md:gap-16 gap-2 flex-col md:flex-row">
            <span class="flex gap-4 md:gap-0 md:flex-col items-center">
                <span class="font-bold">Call</span>
                <a href="tel:0580420563">+966580420563</a>
            </span>
            <span class="flex gap-4 md:gap-0 md:flex-col items-center">
                <span class="font-bold">Email</span>
                <a href="mailto:mohmmadfahad1919@gmail.com">mohmmadfahad1919@gmail.com</a>
            </span>
            <span class="flex items-center">
                <SocialMedia/>
            </span>
        </div>
    </div>
</footer>