<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
  {
    title: "Serious work. Minimal noise.",
    description:
      "We’re security engineers and researchers building autonomous systems that actually find real-world bugs. Not theoretical CVEs. Not lab-replicated exploits. Real code, real software, real impact."
  },
  {
    title: "A product of deep engineering, not marketing",
    description:
      "XBOW isn’t trying to look smart—we’re trying to be effective. We’re applying advanced AI techniques, rigorous program analysis, and practical exploit building to improve how security gets done. The only hype we care about is when a fix goes out before an exploit drops."
  },
  {
    title: "What it's like to work here",
    description:
      "We value people who think independently, work deeply, and take ownership. You’ll have real autonomy—and you’ll be expected to use it. No daily hand-holding. No endless process layers. Just meaningful problems and the room to solve them well."
  },
  {
    title: "We operate on trust",
    description:
      "Everyone on the team has access to sensitive findings as they happen, often before a vendor is even aware. That’s only possible with a high-trust culture and strong ethics. If you want to be looped in, you’d better be accountable."
  },
  {
    title: "Sharp problems. Small team.",
    description:
      "We lean toward highly technical people who care more about accuracy than speed, and who are motivated by solving hard problems that matter. Ship a feature, watch it produce a working exploit, and then see your fingerprint on a patch. We don’t move fast and break things. We move thoroughly and fix them."
  },
  {
    title: "If you're here for the real thing",
    description:
      "This is not a good fit for ‘move fast, learn a little, and jump to the next thing.’ But if you’re someone who wants to work on technically deep tools with high stakes and real-world adoption—not clicky demos—you'll probably enjoy it here. We’re always open to talking to thoughtful, mission-driven technical people. If that’s you, reach out directly. No need to wait for a job post."
  }
];
</script>

<SecondaryHero
	title="Autonomous exploitation. Real risk found."
	subtitle="XBOW uses AI to find and prove critical vulnerabilities—before attackers can."
	imageSrc="/mockups/airport-screen-1747852179412.png"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
  stakeholderType="team"
  title="Elite talent. Proven impact."
  subtitle="Led by experts in security and AI."
  stakeholders={[
    {
      name: "Nico Waisman",
      position: "Head of Security",
      bio: "Internationally recognized security leader and vulnerability expert.",
      image: "/generated/image-a-professional-headshot-of-a-male-securi.webp"
    },
    {
      name: "Brendan Dolan-Gavitt",
      position: "AI Researcher",
      bio: "Professor, researcher, and leading authority in AI-driven security.",
      image: "/generated/image-a-professional-headshot-of-a-male-ai-res.webp"
    }
  ]}
/>

<!-- No investors listed for XBOW -->

<!-- CTA Section -->
<CallToAction
  title="Work on the real problems"
  subtitle="Security, not hype."
  description="Open source powers the systems we depend on—and it still ships critical bugs. XBOW is building autonomous technology that finds and proves real, exploitable vulnerabilities in actual software. No manual tuning. No guesswork. Just verifiable exploit chains that stand on their own."
  callsToAction={[
    { href: '/waitlist', label: 'Join the waitlist', variant: 'primary' },
    { href: 'mailto:team@xbow.ai', label: 'Contact the team', variant: 'secondary' },
    { href: '/updates', label: 'Follow technical updates', variant: 'ghost' }
  ]}
/>
