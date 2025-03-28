<script lang="ts">
	import { AppHeader } from '$lib';
</script>

<AppHeader />

<main class="flex-1 pt-16 md:pt-20 pb-12 w-full">
	<div class="container px-3 md:px-4 py-4 md:py-6 mx-auto max-w-6xl">
		<div>
			<section class="pt-32 pb-20 px-4 relative overflow-hidden" id="hero">
				<div class="absolute inset-0 bg-gradient-to-br from-primary/5 to-secondary/5 z-0"></div>
				<div
					class="absolute top-20 left-10 w-64 h-64 bg-primary/10 rounded-full filter blur-3xl"
				></div>
				<div
					class="absolute bottom-10 right-10 w-72 h-72 bg-secondary/10 rounded-full filter blur-3xl"
				></div>
				<div class="container mx-auto relative z-10">
					<div class="flex flex-col lg:flex-row items-center justify-between gap-12">
						<div class="max-w-xl p-8">
							<span class="chip-primary mb-4 animate-fade-in">Companion AI for Healthcare</span>
							<h1 class="text-4xl font-bold mt-2 mb-4">
								Your Personal Health Companion, Always By Your Side
							</h1>
							<p class="subtitle mt-4 mb-8 animate-fade-in animate-delay-200">
								HealthCompanion AI provides compassionate support, real-time monitoring, and
								personalized care for those who need it most.
							</p>
							<div class="flex flex-wrap gap-4 animate-fade-in animate-delay-300">
								<a
									class="bg-primary hover:bg-primary-dark text-white px-6 py-3 rounded-lg font-medium transition-colors shadow-sm flex items-center"
									href="/en-us/login"
									>Get Started <svg
										xmlns="http://www.w3.org/2000/svg"
										width="18"
										height="18"
										viewBox="0 0 24 24"
										fill="none"
										stroke="currentColor"
										stroke-width="2"
										stroke-linecap="round"
										stroke-linejoin="round"
										class="lucide lucide-arrow-right ml-2"
										><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg
									></a
								><a
									class="bg-base-100 border border-base-content/15 px-6 py-3 rounded-lg font-medium transition-colors hover:bg-gray-50 shadow-sm text-base-content"
									href="/en-us/login">Talk to AI Companion</a
								>
							</div>
						</div>
						<div class="relative w-72 h-72 animate-fade-in animate-delay-200">
							<div class="absolute inset-0 rounded-full bg-primary/5 animate-pulse-slow"></div>
							<div
								class="relative mx-auto rounded-full bg-gradient-to-br from-primary to-primary-dark animate-float w-40 h-40 scale-105 transition-transform duration-1000"
							>
								<div class="absolute inset-1 bg-white rounded-full"></div>
								<div
									class="absolute inset-[5px] bg-gradient-to-br from-primary-light to-primary rounded-full flex items-center justify-center"
								>
									<span class="text-white font-bold text-2xl">AI</span>
								</div>
								<span
									class="absolute bottom-0 right-0 w-4 h-4 bg-success rounded-full border-2 border-white"
								></span>
								<div
									class="absolute inset-[-8px] rounded-full border border-primary/20 transition-opacity duration-1000 opacity-100"
								></div>
								<div
									class="absolute inset-[-16px] rounded-full border border-primary/10 transition-opacity duration-1000 delay-100 opacity-100"
								></div>
							</div>
						</div>
					</div>
				</div>
			</section>
			<section class="py-20 px-4" id="features">
				<div class="container mx-auto">
					<div
						class="text-center max-w-3xl mx-auto mb-16 reveal opacity-0 animate-slide-up opacity-100"
					>
						<span class="chip-secondary mb-4">How We Help</span>
						<h2 class="heading-2">Comprehensive Support Through Technology</h2>
						<p class="subtitle mt-4">
							HealthCompanion AI combines AI, monitoring technology, and human-centered design to
							provide care that is both effective and compassionate.
						</p>
					</div>
					<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
						<div class="glass-card p-6 reveal opacity-0 animate-slide-up opacity-100">
							<div class="w-12 h-12 rounded-lg bg-primary/10 flex items-center justify-center mb-4">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-heart text-primary"
									><path
										d="M19 14c1.49-1.46 3-3.21 3-5.5A5.5 5.5 0 0 0 16.5 3c-1.76 0-3 .5-4.5 2-1.5-1.5-2.74-2-4.5-2A5.5 5.5 0 0 0 2 8.5c0 2.3 1.5 4.05 3 5.5l7 7Z"
									></path></svg
								>
							</div>
							<h3 class="text-xl font-semibold mb-2">Wellness Monitoring</h3>
							<p class="text-muted-foreground">
								Discreet tracking of vital health metrics with personalized insights and timely
								alerts.
							</p>
						</div>
						<div class="glass-card p-6 reveal opacity-0 animate-slide-up opacity-100">
							<div
								class="w-12 h-12 rounded-lg bg-secondary/10 flex items-center justify-center mb-4"
							>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-message-square-heart text-secondary"
									><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"
									></path><path
										d="M14.8 7.5a1.84 1.84 0 0 0-2.6 0l-.2.3-.3-.3a1.84 1.84 0 1 0-2.4 2.8L12 13l2.7-2.7c.9-.9.8-2.1.1-2.8"
									></path></svg
								>
							</div>
							<h3 class="text-xl font-semibold mb-2">Emotional Support</h3>
							<p class="text-muted-foreground">
								Compassionate AI companion available 24/7 for conversation, encouragement, and
								mental wellness.
							</p>
						</div>
						<div class="glass-card p-6 reveal opacity-0 animate-slide-up opacity-100">
							<div class="w-12 h-12 rounded-lg bg-neutral/20 flex items-center justify-center mb-4">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-activity text-neutral-dark"
									><path
										d="M22 12h-2.48a2 2 0 0 0-1.93 1.46l-2.35 8.36a.25.25 0 0 1-.48 0L9.24 2.18a.25.25 0 0 0-.48 0l-2.35 8.36A2 2 0 0 1 4.49 12H2"
									></path></svg
								>
							</div>
							<h3 class="text-xl font-semibold mb-2">Activity Tracking</h3>
							<p class="text-muted-foreground">
								Smart monitoring of daily activities with gentle reminders and encouragement.
							</p>
						</div>
						<div class="glass-card p-6 reveal opacity-0 animate-slide-up opacity-100">
							<div class="w-12 h-12 rounded-lg bg-primary/10 flex items-center justify-center mb-4">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-clock text-primary"
									><circle cx="12" cy="12" r="10"></circle><polyline points="12 6 12 12 16 14"
									></polyline></svg
								>
							</div>
							<h3 class="text-xl font-semibold mb-2">Medication Management</h3>
							<p class="text-muted-foreground">
								Smart medication reminders and tracking to ensure proper dosage and timing for
								better health outcomes.
							</p>
						</div>
						<div class="glass-card p-6 reveal opacity-0 animate-slide-up opacity-100">
							<div
								class="w-12 h-12 rounded-lg bg-secondary/10 flex items-center justify-center mb-4"
							>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-brain text-secondary"
									><path
										d="M12 5a3 3 0 1 0-5.997.125 4 4 0 0 0-2.526 5.77 4 4 0 0 0 .556 6.588A4 4 0 1 0 12 18Z"
									></path><path
										d="M12 5a3 3 0 1 1 5.997.125 4 4 0 0 1 2.526 5.77 4 4 0 0 1-.556 6.588A4 4 0 1 1 12 18Z"
									></path><path d="M15 13a4.5 4.5 0 0 1-3-4 4.5 4.5 0 0 1-3 4"></path><path
										d="M17.599 6.5a3 3 0 0 0 .399-1.375"
									></path><path d="M6.003 5.125A3 3 0 0 0 6.401 6.5"></path><path
										d="M3.477 10.896a4 4 0 0 1 .585-.396"
									></path><path d="M19.938 10.5a4 4 0 0 1 .585.396"></path><path
										d="M6 18a4 4 0 0 1-1.967-.516"
									></path><path d="M19.967 17.484A4 4 0 0 1 18 18"></path></svg
								>
							</div>
							<h3 class="text-xl font-semibold mb-2">Cognitive Engagement</h3>
							<p class="text-muted-foreground">
								Brain-stimulating activities and conversations designed to maintain cognitive
								function and mental acuity.
							</p>
						</div>
						<div class="glass-card p-6 reveal opacity-0 animate-slide-up opacity-100">
							<div class="w-12 h-12 rounded-lg bg-neutral/20 flex items-center justify-center mb-4">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-shield text-neutral-dark"
									><path
										d="M20 13c0 5-3.5 7.5-7.66 8.95a1 1 0 0 1-.67-.01C7.5 20.5 4 18 4 13V6a1 1 0 0 1 1-1c2 0 4.5-1.2 6.24-2.72a1.17 1.17 0 0 1 1.52 0C14.51 3.81 17 5 19 5a1 1 0 0 1 1 1z"
									></path></svg
								>
							</div>
							<h3 class="text-xl font-semibold mb-2">Family Connection</h3>
							<p class="text-muted-foreground">
								Keep family members informed and connected with easy updates and communication
								tools.
							</p>
						</div>
					</div>
				</div>
			</section>
			<section class="py-20 px-4 bg-gradient-to-br from-primary/10 to-secondary/10">
				<div class="container mx-auto">
					<div
						class="max-w-4xl mx-auto glass-card p-8 md:p-12 relative overflow-hidden reveal opacity-0 animate-slide-up opacity-100"
					>
						<div
							class="absolute top-0 right-0 w-64 h-64 bg-primary/10 rounded-full -translate-y-1/2 translate-x-1/2 filter blur-3xl"
						></div>
						<div class="relative">
							<h2 class="heading-2 mb-4">Ready to Experience HealthCompanion AI?</h2>
							<p class="subtitle mb-8 max-w-2xl">
								Join thousands of families who trust HealthCompanion AI for compassionate care and
								monitoring. Start your journey today.
							</p>
							<div class="flex flex-wrap gap-4">
								<a
									class="bg-primary hover:bg-primary-dark text-white px-6 py-3 rounded-lg font-medium transition-colors shadow-sm flex items-center"
									href="/en-us/login"
									>Get Started <svg
										xmlns="http://www.w3.org/2000/svg"
										width="18"
										height="18"
										viewBox="0 0 24 24"
										fill="none"
										stroke="currentColor"
										stroke-width="2"
										stroke-linecap="round"
										stroke-linejoin="round"
										class="lucide lucide-arrow-right ml-2"
										><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg
									></a
								><a
									class="bg-white dark:bg-gray-800 border border-gray-200 dark:border-gray-700 px-6 py-3 rounded-lg font-medium transition-colors hover:bg-gray-50 dark:hover:bg-gray-700 shadow-sm text-foreground"
									href="/en-us/login">Try Demo</a
								>
							</div>
						</div>
					</div>
				</div>
			</section>
		</div>
	</div>
</main>
