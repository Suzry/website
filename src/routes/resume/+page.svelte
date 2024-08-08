<script>

    import ResumeCard from "$lib/components/ResumeCard.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    import Title from "$lib/components/Title.svelte"
    import Container from "$lib/components/Container.svelte"
</script>

<Container>
    <Title title="Resume"/>
    <div class="pt-16 flex flex-col gap-8">
        <div class="flex justify-between items-center">
            <span class="text-2xl font-bold">Education</span>
            <Button>Download CV</Button>
        </div>
        <ResumeCard
         date="2023 - present"
         title="Software Engineering Bachelor"
         company="Umm Al-Qura University">
         Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem aliquam blanditiis cum, cupiditate minus temporibus facilis totam necessitatibus repellat in doloribus odio officia magni repudiandae provident ad quae reiciendis. Veniam?
        </ResumeCard>
    </div>
</Container>