<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ BUILD WITH CONTEXT ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				The workflow engine for AI development.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-lg">
				Devplan bridges the gap between product thinking and AI execution with codebase-aware specs.
			</p>
		</div>
		
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			Book a Demo ->
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ LIVING PROJECTS ]"
			title="Deep product and<br>codebase context"
			description="Maintain a single source of truth with context that stays in sync with your codebase and product decisions."
			tagColor="bg-primary-600"
			tagIcon="arrow"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=Living+Projects+UI"
		/>
		
		<FeatureCard 
			subtitle="[ GUIDED EXECUTION ]"
			title="Deliver specs directly<br>to AI coding agents"
			description="MCP server integration delivers context-rich specs to Cursor, Claude Code, and other AI tools."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=MCP+Integration+UI"
		/>
		
		<FeatureCard 
			subtitle="[ TEAM PLANNING ]"
			title="Auto-estimated timelines<br>with Monte Carlo"
			description="Get realistic project timelines with Monte Carlo estimation based on your team's actual velocity."
			tagColor="bg-accent-pink"
			tagIcon="arrow"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=Timeline+Estimation+UI"
		/>
		
		<FeatureCard 
			subtitle="[ SMART INTAKE ]"
			title="Anyone can submit ideas<br>that AI refines"
			description="Let your team submit rough ideas that Devplan's AI agent automatically refines into detailed specs."
			tagColor="bg-accent-yellow"
			tagIcon="plus"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=Smart+Intake+UI"
		/>
	</div>
</section>
