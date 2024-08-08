<script lang="ts">
    import Container from "$lib/components/Container.svelte";
    import ProjectCard from "$lib/components/ProjectCard.svelte";
    import Title from "$lib/components/Title.svelte";
    import Button from "$lib/components/ui/button/button.svelte"
    
    
</script>
<title> Mohammed </title>

<Container class="flex flex-col gap-16">
    <Title title="Project"/>

    <ProjectCard title="Calculator" subtitle=""  imageSrc="/ProjectPicture.png">
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae minus cumque sit mollitia voluptatum eligendi vero sapiente deserunt recusandae quia facere consectetur quisquam fugiat et, possimus rem quidem odit nam.
        </p>
        <Button class="mt-4" href="https://melodic-dolphin-3a4c8b.netlify.app/" target="_blank">Give it a shot</Button>
    </ProjectCard>

</Container>