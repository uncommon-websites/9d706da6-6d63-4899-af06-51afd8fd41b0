<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Find bugs before attackers do."
	subtitle="Get real vulnerabilities in real software. Automatically."
	imageSrc="/generated/image-a-group-of-cybersecurity-professionals-i.webp"
	centered={false}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/ibm.com',
		'https://logo.clearbit.com/cisco.com',
		'https://logo.clearbit.com/siemens.com',
		'https://logo.clearbit.com/roblox.com'
	]}
/>

<Summary
	title="Autonomous vulnerability discovery, proven in the real world"
	text="XBOW is an AI that autonomously finds and proves actual vulnerabilities in open-source software. It doesn’t just report bugs—it demonstrates real exploits, helping organizations secure what matters most."
/>

<Testimonials
	testimonials={[
		{
			name: "Lukas Schenk",
			position: "Security Engineer",
			company: "Argonix AG",
			quote:
				"XBOW flagged two actual vulnerabilities and proved exploitation within hours—saving us days of triage and giving us clear, actionable results. The time we got back means we can focus on strengthening our entire stack, not chasing false alarms.",
			image:
				"/generated/image-a-male-security-engineer-in-a-modern-off.webp"
		},
		{
			name: "Mei-Lien Wu",
			position: "CTO",
			company: "Bright Startup",
			quote:
				"XBOW uncovered a risk we missed during our internal review. Their exploit proof made it clear what was at stake—now our investors know we take security seriously, and our risk profile has never been better.",
			image:
				"/generated/image-a-female-cto-in-a-tech-startup-workspace.webp"
		},
		{
			name: "Jasper Edel",
			position: "IT Manager",
			company: "Fleetwood Enterprises",
			quote:
				"Automated testing with XBOW helped us avoid a costly retroactive patch. By catching high-impact bugs before our quarterly release, we saved thousands on remediation and compliance headaches.",
			image:
				"/generated/image-a-male-it-manager-in-a-medium-sized-ente.webp"
		}
	]}
/>

<Features
	title="What sets xbow apart"
	subtitle="Each feature is designed for the harsh realities of modern software security."
	features={[
		{
			title: "Autonomous bug discovery",
			description: "XBOW finds vulnerabilities in any software without rules, signatures, or manual tuning."
		},
		{
			title: "Proof, not just detection",
			description: "Each bug comes with working exploitation and secret extraction, showing real risk, not guesswork."
		},
		{
			title: "Responsible real-world impact",
			description: "XBOW reports vulnerabilities directly to vendors after discovery, supporting responsible open source security."
		},
		{
			title: "Multi-layered attack techniques",
			description: "Combines code analysis, disassembly and fuzzing for unmatched vulnerability coverage across stacks."
		},
		{
			title: "Proven success in critical systems",
			description: "XBOW has uncovered and exploited severe CVEs in widely used software like Scoold, benefiting real companies."
		},
		{
			title: "Built for scaling security",
			description: "Empower security teams, vendors, and bug bounty platforms to find and fix risks autonomously at scale."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Secure open-source dependencies",
			description: "Proactively identify and prove real vulnerabilities in the open-source components your organization depends on—before they put your business at risk.",
			image: "/generated/image-a-diverse-security-team-gathered-around-.webp",
			link: {
				href: "/use-cases/open-source-security",
				label: "Learn more"
			}
		},
		{
			title: "Ship trusted software releases",
			description: "Automatically test new builds for exploitable bugs, so vendors can release updates with confidence and minimize emergency patches.",
			image: "/generated/image-a-group-of-software-developers-in-a-cont.webp",
			link: {
				href: "/use-cases/secure-releases",
				label: "Learn more"
			}
		},
		{
			title: "Scale bug bounty efficiency",
			description: "Empower bug bounty programs with autonomous vulnerability discovery—enabling researchers to focus on verification and high-priority fixes, not repetitive triage.",
			image: "/generated/image-a-team-of-professional-bug-bounty-resear.webp",
			link: {
				href: "/use-cases/bug-bounty-automation",
				label: "Learn more"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction
  title="AI that spots real vulnerabilities before attackers do"
  subtitle="Autonomous security that proves the risk—before it costs you."
  description="XBOW autonomously finds and proves software exploits—saving security teams hours of triage and reducing risk across your stack. It’s already uncovered high-impact bugs in real-world systems trusted by Cisco, IBM, and others."
  imageSrc="/generated/image-a-smiling-security-engineer-in-a-bustlin.webp"
  callsToAction={[
    { href: '/waitlist', label: 'Join the waitlist', variant: 'primary' },
    { href: '/contact', label: 'Request a demo', variant: 'secondary' }
  ]}
/>
