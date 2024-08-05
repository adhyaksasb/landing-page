<script>
	import '../app.css';
	import Sidebar from '$lib/components/Navbar/Sidebar.svelte';
	import Header from '$lib/components/Navbar/Header.svelte';
	import LandingSidebar from '$lib/components/Landing/LandingSidebar.svelte';

	import { Send, Phone, Building2, Linkedin, Instagram, Facebook } from 'lucide-svelte';
	let logo = '/assets/images/rectangle.png';
	import { page } from '$app/stores';

	let { children } = $props();

	import { ModeWatcher } from 'mode-watcher';
	let path = $derived($page.url.pathname);
</script>

<ModeWatcher></ModeWatcher>
<div class="grid h-[95vh] w-full grid-cols-12 rounded-xl py-4 pr-4">
	<div class="col-span-3 h-[95vh]">
		<div class="grid h-[95vh] w-full grid-rows-2">
			<div class="flex items-center justify-center">
				<img src={logo} alt="" />
			</div>
			<div class="flex flex-col items-center px-6">
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
	</div>
	<div class="col-span-9 h-[95vh] rounded-xl bg-[url('/assets/images/background.png')] bg-center">
		<div class="flex flex-col">
			<div class="flex flex-row-reverse">
				<div class="h-10 w-16 rounded-bl-xl bg-background">B</div>
				<div class="w-full rounded-t-xl">gdfgfd</div>
			</div>
			<div class="grid h-[92vh] grid-rows-12">
				<div class="row-span-9 h-full">gdfgd</div>
				<div class="row-span-3 h-full">
					<div class="grid grid-cols-4">
						<div class="col-span-1 h-[22vh] w-full rounded-xl border-[20px] border-background">
							gdfgdfgdfgdf
						</div>
						<div class="col-span-3 w-full">fdgfdgfdgdfgdf</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
