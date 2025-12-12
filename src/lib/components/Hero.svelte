<script lang="ts">
	// Integration logos
	const logos = [
		{ name: 'GitHub', width: 80 },
		{ name: 'Linear', width: 90 },
		{ name: 'Jira', width: 60 },
		{ name: 'Cursor', width: 80 },
		{ name: 'Claude', width: 90 },
		{ name: 'Windsurf', width: 80 },
		{ name: 'Bitbucket', width: 100 },
		{ name: 'v0', width: 60 },
		{ name: 'Bolt', width: 70 },
		{ name: 'MCP', width: 60 }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-gray-900 leading-[0.9] tracking-tight mb-8">
				Context-Rich Specs for AI Development
			</h1>
			
			<div class="relative w-12 h-12 mb-8">
				<!-- Plan icon -->
				<svg viewBox="0 0 24 24" fill="none" class="w-8 h-8 text-primary-500 absolute top-0 left-0">
					<rect x="3" y="3" width="18" height="18" rx="2" stroke="currentColor" stroke-width="2" fill="none"/>
					<path d="M8 7h8M8 12h8M8 17h4" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
				</svg>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="font-mono text-sm text-gray-700 uppercase tracking-wider leading-relaxed">
					Generate detailed specs from your<br>
					codebase and product data to guide<br>
					AI coding agents with zero hallucinations
				</p>

				<div class="flex flex-col items-start gap-3">
					<button class="bg-primary-600 text-white px-6 py-3 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2">
						Start Free Trial 
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</button>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						14-day free trial - no credit card required
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<!-- Spec generation visualization -->
			<div class="absolute inset-0 flex items-center justify-center opacity-90">
				<div class="w-full h-full max-w-lg mx-auto p-8">
					<!-- Simplified spec document illustration -->
					<div class="bg-white border-2 border-gray-300 rounded-lg shadow-2xl p-6 space-y-4 transform rotate-2">
						<div class="h-3 bg-primary-200 rounded w-3/4"></div>
						<div class="h-3 bg-gray-200 rounded w-full"></div>
						<div class="h-3 bg-gray-200 rounded w-5/6"></div>
						<div class="h-8 bg-gray-100 rounded mt-6"></div>
						<div class="space-y-2">
							<div class="h-2 bg-gray-200 rounded w-full"></div>
							<div class="h-2 bg-gray-200 rounded w-full"></div>
							<div class="h-2 bg-gray-200 rounded w-4/5"></div>
						</div>
					</div>
					<div class="bg-white border-2 border-gray-300 rounded-lg shadow-xl p-6 space-y-4 transform -rotate-3 -mt-32 ml-16">
						<div class="h-3 bg-primary-300 rounded w-2/3"></div>
						<div class="h-3 bg-gray-200 rounded w-full"></div>
						<div class="h-3 bg-gray-200 rounded w-3/4"></div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-300 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-600 mb-6">
			Now live in beta - Integrates with your dev tools
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-5 gap-8 opacity-60 grayscale">
			{#each logos as logo}
				<div class="h-8 flex items-center justify-center border border-gray-300/50 rounded bg-gray-100/50">
					<span class="text-xs font-bold text-gray-500">{logo.name}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
