<script>
    import ThemeSwitch from "$lib/components/themeSwitch.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    import { Title } from "$lib/components/ui/sheet";
    import SocialMedia from "$lib/components/SocialMedia.svelte"
</script>

<title> Mohammed </title>

<div class="flex justify-end pb-[35rem] lg:pb-0 ">
    <div
        class="bg-secondary text-secondary-foreground relative  w-full lg:w-[60vw] min-h-[40vh] lg:min-h-[calc(100dvh-10.5rem)] flex justify-center items-center pb-32"
    >
        <div
            class=" bg-[#f4ece6] dark:bg-[#303030] shadow-[0_10px_60px_-15px_rgba(0,0,0,0.7)] dark:shadow-[0_10px_60px_-15px_rgba(0,0,0,0.7)] w-[22rem] absolute lg:start-10 lg:-translate-x-full  items-center flex flex-col justify-between pt-8 gap-2 self-bottom lg:self-start  translate-y-[105%] lg:translate-y-[10%] max-w-[80dw]"
        >
            <img
                src="https://media-pmo1-1.cdn.whatsapp.net/v/t61.24694-24/408169282_234811572970656_4218674785800751800_n.jpg?ccb=11-4&oh=01_Q5AaIIQGAvatrtmCGnkVGJrg9g1mojOvF_kxHCdz_BvnaaYG&oe=66BE496E&_nc_sid=5e03e0&_nc_cat=101"
                class="rounded-full w-64 mx-auto"
                alt="الصورة الشخصية"
            />
            <div class=" flex flex-col items-center gap-8">
                <h1 class=" font-bold text-4xl">Mohammed</h1>
                <hr class=" w-24 border-2 border-primary " />
                <h2 class="text-2xl">Web Developer</h2>
            </div>
            <div
                class="bg-secondary text-secondary-foreground w-full flex justify-center p-2 mt-12 gap-5"
            >
                <SocialMedia/>
            </div>
        </div>
        <div class=" mx-10 max-w-[30rem] flex flex-col gap-8">
            <h1 class="text-8xl font-extrabold">Hello
            </h1>
            <h4 class="text-4xl font-semibold">
                Here's who I am & what I do
            </h4>
            <div class="flex gap-2">
                <Button class="w-32" href="/resume">
                    Resume
                </Button>
                <Button class="w-32" variant="outline"  href = "/projects">
                    Projects
                </Button>
            </div>
            <div>
                <p class="font-semibold">
                    I am a first-year Software Engineering student at Umm Al-Qura University. I have a strong passion for technology and software development, constantly seeking to enhance my technical skills through academic and personal projects. I enjoy teamwork and collaborating with my peers on innovative solutions to technical challenges. I aspire to contribute to the development of software that improves quality of life and simplifies daily tasks for people.
                </p>
            </div>
        </div>
    </div>
</div>
