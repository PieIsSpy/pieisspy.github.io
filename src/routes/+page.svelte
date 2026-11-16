<script>
	import * as Avatar from '#lib/components/ui/avatar/index.ts';
	import Badge from '#lib/components/ui/badge/badge.svelte';
    import { Button } from '#lib/components/ui/button/index.ts';
</script>

<div class="flex items-center justify-center gap-3 rounded-lg border bg p-6 text-card-foreground shadow-sm">
    <Avatar.Root class="h-40 w-40">
        <Avatar.Image src="https://github.com/pieisspy.png" alt="Profile"/>
        <Avatar.Fallback>GH</Avatar.Fallback>
    </Avatar.Root>
    <div>
        <h2 class="text-2xl font-bold tracking-tight">PieIsSpy</h2>
        <p>Hello! I am PieIsSpy! I am a QA Engineer and Usability Tester who is also passionate in Animations!</p>
        <div>
            <a class="text-sm font-medium underline underline-offset-4 hover:text-primary" href="https://www.linkedin.com/in/karl-deejay-omandac-470203434">LinkedIn</a>
            <a class="text-sm font-medium underline underline-offset-4 hover:text-primary" href="https://github.com/PieIsSpy">Github</a>
        </div>
        <Button href='/resume.pdf' size="sm" class="rounded-sm margin">Resume</Button>
    </div>
</div>

<div>
    <div class="mx-auto flex w-full max-w-2xl flex-col gap-6 px-4 py-12">
        <h3 class="text-lg font-semibold tracking-tight mb-3">Skills</h3>
        <div>
            <p>Languages:</p>
            <Badge variant="secondary">C</Badge>
            <Badge variant="secondary">Java</Badge>
            <Badge variant="secondary">Python</Badge>
            <Badge variant="secondary">Typescript</Badge>
        </div>

        <div>
            <p>Frontend:</p>
            <Badge variant="secondary">HTML/CSS</Badge>
            <Badge variant="secondary">React</Badge>
            <Badge variant="secondary">Svelte</Badge>
        </div>

        <div>
            <p>Tools:</p>
            <Badge variant="secondary">Git</Badge>
            <Badge variant="secondary">Github</Badge>
            <Badge variant="secondary">Npm</Badge>
        </div>
    </div>

    <div class="mx-auto flex w-full max-w-2xl flex-col gap-6 px-4 py-12">
        <h3 class="text-lg font-semibold tracking-tight mb-3">Education</h3>
        <div>
            <div class="flex justify-between">
                <p class="font-semibold">De La Salle University - Manila</p>
                <p class="font-light">Expected 2028</p>
            </div>
            <p>Bachelor in Science in Computer Science, Major in Software Technology</p>
        </div>
    </div>

    <div class="mx-auto flex w-full max-w-2xl flex-col gap-6 px-4 py-12">
        <h3 class="text-lg font-semibold tracking-tight mb-3">Experience</h3>
        <div>
            <div class="flex justify-between">
                <p class="font-semibold">Slottle</p>
                <p class="font-light">2026</p>
            </div>
            <p>QA and Usability Tester</p>
        </div>
    </div>
</div>