<section class="bg-primary-50 py-24 px-6 md:px-12 relative overflow-hidden">
	<div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-600 uppercase tracking-widest mb-4 block">
				[ BUILD WITH CONTEXT, NOT HALLUCINATIONS ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Codebase-Aware<br>Spec Generation
			</h2>
			<p class="font-mono text-sm text-gray-700 max-w-md mb-8 leading-relaxed">
				Devplan analyzes your codebase to generate specs that understand your architecture, patterns, and dependencies. AI agents get the context they need to ship quality code.
			</p>
			
			<button class="bg-primary-600 text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				Learn more ->
			</button>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- Codebase Analysis Visualization -->
			<div class="absolute inset-0">
				<svg width="100%" height="100%" viewBox="0 0 400 300" class="overflow-visible">
					<!-- Nodes representing codebase components -->
                    <g fill="oklch(0.627 0.194 149.214)" stroke="#fff" stroke-width="1">
                        <circle cx="200" cy="150" r="6" />
                        <circle cx="150" cy="100" r="4" />
                        <circle cx="250" cy="100" r="4" />
                        <circle cx="150" cy="200" r="4" />
                        <circle cx="250" cy="200" r="4" />
                        <circle cx="100" cy="150" r="3" />
                        <circle cx="300" cy="150" r="3" />
                        
                        <!-- Additional nodes -->
                        <circle cx="180" cy="80" r="3" />
                        <circle cx="220" cy="80" r="3" />
                        <circle cx="180" cy="220" r="3" />
                        <circle cx="220" cy="220" r="3" />
                    </g>
                    
                    <!-- Edges showing relationships -->
                    <g stroke="oklch(0.627 0.194 149.214)" stroke-width="0.5" opacity="0.6">
                        <line x1="200" y1="150" x2="150" y2="100" />
                        <line x1="200" y1="150" x2="250" y2="100" />
                        <line x1="200" y1="150" x2="150" y2="200" />
                        <line x1="200" y1="150" x2="250" y2="200" />
                        <line x1="150" y1="100" x2="100" y2="150" />
                        <line x1="250" y1="100" x2="300" y2="150" />
                        <line x1="150" y1="200" x2="100" y2="150" />
                        <line x1="250" y1="200" x2="300" y2="150" />
                        <line x1="150" y1="100" x2="180" y2="80" />
                        <line x1="250" y1="100" x2="220" y2="80" />
                    </g>
				</svg>
			</div>
		</div>
	</div>
    
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-10" 
        style="background-image: linear-gradient(#000 1px, transparent 1px), linear-gradient(90deg, #000 1px, transparent 1px); background-size: 40px 40px;">
    </div>
</section>
