<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "How does Devplan pricing work?",
			answer: "Devplan offers a Builder plan at $24/month for individuals, and a Team plan at $49/month for up to 3 users ($19 per additional user). Enterprise plans with custom pricing are also available."
		},
		{
			question: "What integrations does Devplan support?",
			answer: "Devplan integrates with GitHub, GitLab, Bitbucket, Linear, Jira, Cursor, Windsurf, Claude Code, v0, Bolt, and includes an MCP server for delivering specs to AI coding agents."
		},
		{
			question: "Is there a free trial available?",
			answer: "Yes, we offer a 14-day free trial with no credit card required. You get full access to all features during the trial period."
		},
		{
			question: "How does Devplan analyze my codebase?",
			answer: "Devplan scans your repositories to understand your architecture, patterns, and dependencies. This context is used to generate specs that are aligned with your existing codebase."
		},
		{
			question: "Can Devplan work with my existing workflow?",
			answer: "Yes, Devplan is designed to integrate seamlessly with your existing tools. It works alongside Linear, Jira, and your favorite AI coding tools through our MCP server integration."
		},
		{
			question: "What's the difference between Devplan and traditional PRD tools?",
			answer: "Unlike traditional PRD tools, Devplan generates context-rich specs specifically designed for AI coding agents. It understands your codebase and creates specifications that prevent AI hallucinations."
		},
		{
			question: "How long does it take to get started?",
			answer: "Most teams are up and running in less than a day. Simply connect your repositories, and Devplan will start analyzing your codebase to provide context-aware spec generation."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<button class="bg-primary-600 text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</button>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="font-mono text-sm font-medium text-gray-800 group-hover:text-primary-600 transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl font-mono">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
