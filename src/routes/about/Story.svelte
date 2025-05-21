<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";

	let {
	paragraphs = [
		"XBOW started with a simple question: can AI do more than just spot weak points—can it actually hunt down and prove critical software bugs by itself? The answer moved quickly from research to reality. When XBOW outperformed standard benchmarks, we sent it after real-world open-source projects where the risks are bigger and the stakes are real.",
		"In the field, XBOW proved its strength. It found—and exploited—a severe vulnerability in Scoold, an open-source Q&A platform used by brands like IBM and Siemens. We worked with developers and vendors to get it fixed before it could be weaponized. Each discovery moves open source security forward, protecting everyone who relies on this shared code.",
		"Today, security teams, vendors, and bug bounty programs depend on XBOW to stay ahead of threats. There's no manual tuning or stacks of alerts. It’s real, autonomous security—from reading code to proving risk exists—helping make the world’s technology safer, one vulnerability at a time."
	]
}: {
	paragraphs: string[];
} = $props();
</script>

<div class="">
	<article class="section-py container mx-auto grid max-w-full">
		<Summary text={paragraphs.join("\n\n")} />
	</article>
</div>
