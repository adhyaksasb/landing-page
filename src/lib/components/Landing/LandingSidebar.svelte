<script lang="ts">
	import { Send, Phone, Building2, Linkedin, Instagram, Facebook } from 'lucide-svelte';
	let logo = '/assets/images/rectangle.png';
</script>

<aside
	class="fixed left-0 top-[2.5vh] z-50 hidden h-[95vh] w-[280px] flex-col items-center gap-y-4 bg-background py-5 shadow-lg sm:flex"
>
	<div class="grid h-screen w-full grid-rows-2">
		<div class="flex items-center justify-center">
			<img src={logo} alt="" />
		</div>
		<div class="px-6">
			<div class="mb-10 flex flex-col gap-5">
				<h1 class="text-3xl font-semibold">Let's Talk</h1>
				<div class="flex flex-col gap-4">
					<div class="flex gap-2">
						<Send class="h-6 w-6" />
						<p>rizalmaidanytb@gmail.com</p>
					</div>
					<div class="flex gap-2">
						<Phone class="h-6 w-6" />
						<p>+62 81320718185</p>
					</div>
					<div class="flex items-center gap-2">
						<Building2 class="h-6 w-6" />
						<p>Bandung, Jawa Barat, Indonesia</p>
					</div>
				</div>
			</div>
			<div class="flex gap-4">
				<div class="rounded-sm border border-background p-3">
					<Linkedin class="h-8 w-8" />
				</div>
				<div class="rounded-sm border border-background p-3">
					<Instagram class="h-8 w-8" />
				</div>
				<div class="rounded-sm border border-background p-3">
					<Facebook class="h-8 w-8" />
				</div>
			</div>
		</div>
	</div>
</aside>
