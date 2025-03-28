<script lang="ts">
	export let navItems = [
		{ label: 'Dashboard', url: '#' },
		{ label: 'Health Dashboard', url: '#' },
		{ label: 'Patients', url: '#' },
		{ label: 'Team', url: '#' },
		{ label: 'Calendar', url: '#' },
		{ label: 'Messenger', url: '#' },
		{ label: 'Companion', url: '#' }
	];

	const toggleTheme = () => {
		const htmlElement = document.documentElement;
		const currentTheme = htmlElement.getAttribute('data-theme');

		if (currentTheme === 'dark') {
			htmlElement.setAttribute('data-theme', 'light');
		} else {
			htmlElement.setAttribute('data-theme', 'dark');
		}
	};
</script>

<header
	class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 py-4 px-6 bg-base-100 shadow-sm"
>
	<div class="flex items-center justify-between w-full">
		<div class="flex items-center gap-4">
			<a class="flex items-center" href="/"
				><div class="flex items-center gap-2">
					<div class="relative flex items-center justify-center w-8 h-8">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							fill="#3A7CA5"
							stroke="currentColor"
							stroke-width="1.5"
							stroke-linecap="round"
							stroke-linejoin="round"
							class="lucide lucide-heart absolute text-primary w-7 h-7"
							><path
								d="M19 14c1.49-1.46 3-3.21 3-5.5A5.5 5.5 0 0 0 16.5 3c-1.76 0-3 .5-4.5 2-1.5-1.5-2.74-2-4.5-2A5.5 5.5 0 0 0 2 8.5c0 2.3 1.5 4.05 3 5.5l7 7Z"
							></path></svg
						><svg
							xmlns="http://www.w3.org/2000/svg"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							fill="none"
							stroke="currentColor"
							stroke-width="2.5"
							stroke-linecap="round"
							stroke-linejoin="round"
							class="lucide lucide-activity absolute text-white w-4 h-4 transform translate-y-[1px]"
							><path
								d="M22 12h-2.48a2 2 0 0 0-1.93 1.46l-2.35 8.36a.25.25 0 0 1-.48 0L9.24 2.18a.25.25 0 0 0-.48 0l-2.35 8.36A2 2 0 0 1 4.49 12H2"
							></path></svg
						>
					</div>
					<span class="font-display text-lg font-medium tracking-tight text-foreground"
						>HealthCompanionAI</span
					>
				</div></a
			>
			<div class="hidden md:flex ml-6">
				<ul class="hidden md:flex items-center space-x-8">
					{#each navItems as { label, url }, i}
						<li>
							<a
								class={i === 0
									? 'font-medium transition-colors hover:text-primary relative py-2 text-primary after:absolute after:bottom-0 after:left-0 after:right-0 after:h-0.5 after:bg-primary after:rounded-full'
									: 'font-medium transition-colors hover:text-primary relative py-2 text-base-content/80'}
								href={url}>{label}</a
							>
						</li>
					{/each}
				</ul>
			</div>
			<button class="md:hidden text-foreground rounded-full p-2 hover:bg-muted/20 transition-colors"
				><svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="lucide lucide-menu"
					><line x1="4" x2="20" y1="12" y2="12"></line><line x1="4" x2="20" y1="6" y2="6"
					></line><line x1="4" x2="20" y1="18" y2="18"></line></svg
				></button
			>
		</div>
		<div class="flex items-center gap-4">
			<button aria-label="Toggle theme button" class="swap swap-rotate" on:click={toggleTheme}>
				<input type="checkbox" class="theme-controller" value="synthwave" />
				<svg
					class="swap-off h-6 w-6 fill-current"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
				>
					<path
						d="M5.64,17l-.71.71a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l.71-.71A1,1,0,0,0,5.64,17ZM5,12a1,1,0,0,0-1-1H3a1,1,0,0,0,0,2H4A1,1,0,0,0,5,12Zm7-7a1,1,0,0,0,1-1V3a1,1,0,0,0-2,0V4A1,1,0,0,0,12,5ZM5.64,7.05a1,1,0,0,0,.7.29,1,1,0,0,0,.71-.29,1,1,0,0,0,0-1.41l-.71-.71A1,1,0,0,0,4.93,6.34Zm12,.29a1,1,0,0,0,.7-.29l.71-.71a1,1,0,1,0-1.41-1.41L17,5.64a1,1,0,0,0,0,1.41A1,1,0,0,0,17.66,7.34ZM21,11H20a1,1,0,0,0,0,2h1a1,1,0,0,0,0-2Zm-9,8a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V20A1,1,0,0,0,12,19ZM18.36,17A1,1,0,0,0,17,18.36l.71.71a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41ZM12,6.5A5.5,5.5,0,1,0,17.5,12,5.51,5.51,0,0,0,12,6.5Zm0,9A3.5,3.5,0,1,1,15.5,12,3.5,3.5,0,0,1,12,15.5Z"
					/>
				</svg>
				<svg
					class="swap-on h-6 w-6 fill-current"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
				>
					<path
						d="M21.64,13a1,1,0,0,0-1.05-.14,8.05,8.05,0,0,1-3.37.73A8.15,8.15,0,0,1,9.08,5.49a8.59,8.59,0,0,1,.25-2A1,1,0,0,0,8,2.36,10.14,10.14,0,1,0,22,14.05,1,1,0,0,0,21.64,13Zm-9.5,6.69A8.14,8.14,0,0,1,7.08,5.22v.27A10.15,10.15,0,0,0,17.22,15.63a9.79,9.79,0,0,0,2.1-.22A8.11,8.11,0,0,1,12.14,19.73Z"
					/>
				</svg>
			</button>

			<button
				class="flex items-center gap-1 rounded-full p-2 transition-colors text-foreground/80 hover:text-foreground hover:bg-foreground/10 dark:text-gray-300 dark:hover:text-white dark:hover:bg-gray-700/50"
				aria-label="Select Language"
				type="button"
				id="radix-:rc:"
				aria-haspopup="menu"
				aria-expanded="false"
				data-state="closed"
				><svg
					xmlns="http://www.w3.org/2000/svg"
					width="20"
					height="20"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="lucide lucide-globe"
					><circle cx="12" cy="12" r="10"></circle><path
						d="M12 2a14.5 14.5 0 0 0 0 20 14.5 14.5 0 0 0 0-20"
					></path><path d="M2 12h20"></path></svg
				><span class="text-xs font-medium uppercase">en</span></button
			>
			<div class="relative">
				<button class="rounded-full bg-primary/10 hover:bg-primary/20 p-2 transition-colors"
					><span
						class="relative flex shrink-0 overflow-hidden rounded-full h-8 w-8 border border-primary/20"
						><span
							class="flex h-full w-full items-center justify-center rounded-full bg-primary/5 text-primary"
							><svg
								xmlns="http://www.w3.org/2000/svg"
								width="16"
								height="16"
								viewBox="0 0 24 24"
								fill="none"
								stroke="currentColor"
								stroke-width="2"
								stroke-linecap="round"
								stroke-linejoin="round"
								class="lucide lucide-user"
								><path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"></path><circle
									cx="12"
									cy="7"
									r="4"
								></circle></svg
							></span
						></span
					></button
				>
			</div>
		</div>
	</div>
</header>
