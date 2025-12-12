<script lang="ts">
	const testimonials = [
		{
			quote: "This tool is a game-changer, helping us save tons of time when shaping our app ideas with clarity.",
			author: "Seddick T.",
			role: "Product Leader",
			image: "https://i.pravatar.cc/150?u=seddick",
            icon: "https://placehold.co/20x20/333/fff?text=S"
		},
		{
			quote: "Using Devplan felt like magic... it felt like having an experienced PM working with me.",
			author: "Omar S.",
			role: "Founder",
			image: "https://i.pravatar.cc/150?u=omar",
            icon: "https://placehold.co/20x20/000/fff?text=O"
		},
		{
			quote: "It's really good at giving you a quick glance at edge cases you'll need to cover.",
			author: "Adam L.",
			role: "Tech Solutions Architect",
			image: "https://i.pravatar.cc/150?u=adam",
            icon: "https://placehold.co/20x20/purple/fff?text=A"
		},
		{
			quote: "We are running our 15 person VC-backed company right now without a PM. Devplan helps fills that gap for us... What used to take me days of back and forth and refinement I'm now doing in less than a hour.",
			author: "Andrew N.",
			role: "YC-backed Founder",
			image: "https://i.pravatar.cc/150?u=andrew",
            icon: "https://placehold.co/20x20/blue/fff?text=Y"
		},
		{
			quote: "The conversational collaborative way we are working together on these docs, it really helps tease out the details.",
			author: "Stuart B.",
			role: "Agency Owner",
			image: "https://i.pravatar.cc/150?u=stuart",
            icon: "https://placehold.co/20x20/green/fff?text=S"
		},
		{
			quote: "Pricing is very reasonable for what it offers.",
			author: "George K.",
			role: "Tech Lead",
			image: "https://i.pravatar.cc/150?u=george",
            icon: "https://placehold.co/20x20/red/fff?text=G"
		},
        {
			quote: "Before Devplan I used to run a lot of prompts for Idea --> PRD, PRD --> Tasks, Tasks --> GUI.",
			author: "Alon U.",
			role: "Principal Designer",
			image: "https://i.pravatar.cc/150?u=alon",
            icon: "https://placehold.co/20x20/333/fff?text=A"
		},
        {
			quote: "This is a game changer tool for solo entrepreneurs... I am defining and executing projects much faster with it.",
			author: "Ramy V.",
			role: "Entrepreneur",
			image: "https://i.pravatar.cc/150?u=ramy",
            icon: "https://placehold.co/20x20/orange/fff?text=R"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Loved by Product Teams
		</h2>
		<p class="font-mono text-sm text-gray-600">
			From solo founders to VC-backed companies, teams are shipping faster with Devplan
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm break-inside-avoid hover:shadow-md transition-shadow">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
                    <img src={t.icon} alt="Company Logo" class="w-5 h-5 rounded-sm opacity-70 grayscale" />
				</div>
			</div>
		{/each}
	</div>
</section>
