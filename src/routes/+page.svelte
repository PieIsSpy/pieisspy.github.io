<script>
	import * as Avatar from '#lib/components/ui/avatar/index.ts';
	import { Badge } from '#lib/components/ui/badge/index.ts';
	import { Button } from '#lib/components/ui/button/index.ts';
</script>

<main class="mx-auto flex w-full max-w-2xl flex-col gap-6 px-4 py-12">
	<div class="flex flex-col items-center gap-6 rounded-lg border bg-card p-6 text-card-foreground shadow-sm sm:flex-row sm:items-start">
		<Avatar.Root class="h-32 w-32 shrink-0">
			<Avatar.Image src="https://github.com/pieisspy.png" alt="Profile" />
			<Avatar.Fallback>GH</Avatar.Fallback>
		</Avatar.Root>

		<div class="flex flex-col items-center gap-3 text-center sm:items-start sm:text-left">
			<h2 class="text-2xl font-bold tracking-tight">PieIsSpy</h2>
			<p class="text-sm text-muted-foreground">
				Hello! I am PieIsSpy! I am a QA Engineer and Usability Tester who is also passionate in Animations!
			</p>

			<div class="flex items-center gap-4">
                <a
                    class="text-sm font-medium underline underline-offset-4 hover:text-primary"
                    href="https://www.linkedin.com/in/karl-deejay-omandac-470203434"
                    target="_blank"
                    rel="noreferrer"
                >
                    LinkedIn
                </a>
                <a
                    class="text-sm font-medium underline underline-offset-4 hover:text-primary"
                    href="https://github.com/PieIsSpy"
                    target="_blank"
                    rel="noreferrer"
                >
                    GitHub
                </a>
            </div>

            <div class="pt-1">
                <Button href="/resume.pdf" size="sm" class="rounded-sm">Resume</Button>
            </div>
		</div>
	</div>

	<div class="flex flex-col gap-4 rounded-lg border bg-card p-6 text-card-foreground shadow-sm">
		<h3 class="text-lg font-semibold tracking-tight">Skills</h3>

		<div class="flex flex-col gap-3">
			<div class="flex flex-wrap items-center gap-2">
				<span class="w-24 text-sm font-medium text-muted-foreground">Languages:</span>
				<Badge variant="secondary" class="rounded-sm">C</Badge>
				<Badge variant="secondary" class="rounded-sm">Java</Badge>
				<Badge variant="secondary" class="rounded-sm">Python</Badge>
				<Badge variant="secondary" class="rounded-sm">TypeScript</Badge>
			</div>

			<div class="flex flex-wrap items-center gap-2">
				<span class="w-24 text-sm font-medium text-muted-foreground">Frontend:</span>
				<Badge variant="secondary" class="rounded-sm">HTML/CSS</Badge>
				<Badge variant="secondary" class="rounded-sm">React</Badge>
				<Badge variant="secondary" class="rounded-sm">Svelte</Badge>
			</div>

			<div class="flex flex-wrap items-center gap-2">
				<span class="w-24 text-sm font-medium text-muted-foreground">Tools:</span>
				<Badge variant="secondary" class="rounded-sm">Git</Badge>
				<Badge variant="secondary" class="rounded-sm">GitHub</Badge>
				<Badge variant="secondary" class="rounded-sm">npm</Badge>
			</div>
		</div>
	</div>

	<div class="flex flex-col gap-3 rounded-lg border bg-card p-6 text-card-foreground shadow-sm">
		<h3 class="text-lg font-semibold tracking-tight">Education</h3>
		<div class="flex flex-col gap-1">
			<div class="flex items-baseline justify-between gap-2">
				<p class="font-medium">De La Salle University - Manila</p>
				<p class="text-xs text-muted-foreground">Expected 2028</p>
			</div>
			<p class="text-sm text-muted-foreground">
				Bachelor of Science in Computer Science, Major in Software Technology
			</p>
		</div>
	</div>

	<div class="flex flex-col gap-3 rounded-lg border bg-card p-6 text-card-foreground shadow-sm">
		<h3 class="text-lg font-semibold tracking-tight">Experience</h3>
		<div class="flex flex-col gap-1">
			<div class="flex items-baseline justify-between gap-2">
				<p class="font-medium">Slottle</p>
				<p class="text-xs text-muted-foreground">2026</p>
			</div>
			<p class="text-sm text-muted-foreground">QA and Usability Tester</p>
		</div>
	</div>
</main>