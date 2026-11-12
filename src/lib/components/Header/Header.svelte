<script lang="ts">
	import GithubIcon from '#lib/assets/GithubIcon.svelte';
	import { House, CodeXml, BriefcaseBusiness, Contact, Folders } from '@lucide/svelte';


    import { AppBar } from '@skeletonlabs/skeleton-svelte';
    
</script>

<AppBar class="border-surface-200-800 bg-surface-50-950/75 sticky border-b backdrop-blur-lg top-0 z-50">
    <AppBar.Toolbar class="grid-cols-[auto_1fr_auto] max-w-6xl w-full mx-auto">
        <AppBar.Lead>
            <a href="/" rel="cononical" class="flex gap-x-4 justify-center items-center">
                <CodeXml class="scale-150"/>
                <h1 class="font-semibold text-2xl">Brenny.zip</h1>
            </a>
        </AppBar.Lead>
        <AppBar.Headline>

        </AppBar.Headline>
        <AppBar.Trail>
            <a href="/" class="btn hover:preset-tonal-brand flex">
                <House />
                <p>Home</p>
            </a>
            <a href="/projects" class="btn hover:preset-tonal-brand flex">
                <Folders />
                <p>Projects</p>
            </a>
            <a href="/portfolio" class="btn hover:preset-tonal-brand flex">
                <BriefcaseBusiness />
                <p>Portfolio</p>
            </a>
            <a href="https://github.com/1Brenny1" class="btn hover:preset-tonal-brand flex">
                <GithubIcon />
                <p>Github</p>
            </a>
            <a href="/contact" class="btn hover:preset-tonal-brand flex">
                <Contact />
                <p>Contact</p>
            </a>
        </AppBar.Trail>
    </AppBar.Toolbar>
</AppBar>