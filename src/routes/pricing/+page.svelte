<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Victor Sajan",
      position: "Security Lead",
      company: "Swifteer Inc.",
      quote:
        "As someone who manages a bug bounty program, seeing a fully functioning proof of exploit automatically generated blew me away. XBOW is easy to integrate and the value is clear from day one.",
      image: "/generated/image-professional-headshot-of-a-black-male-ex.webp"
    },
    {
      name: "Laura Shin",
      position: "Director of Product Security",
      company: "Verity Cloud",
      quote:
        "XBOW saved us weeks of manual triage by showing not just that a bug existed—but how it could be fully exploited. Our team sees a clear return on investment.",
      image: "/generated/image-professional-headshot-of-a-south-asian-w.webp"
    },
    {
      name: "Sina Mostaghim",
      position: "VP Engineering",
      company: "Elmora Analytics",
      quote:
        "We use a lot of OSS internally. XBOW’s real-world scanning surfaced critical issues we would’ve otherwise missed, all with minimal setup. The ROI is undeniable.",
      image: "/generated/image-professional-headshot-of-an-east-asian-m.webp"
    }
  ]}
/>

<CallToAction
  title="A faster way to find security flaws in real-world software"
  subtitle="Let XBOW handle the hunt for you"
  description="XBOW autonomously uncovers and proves real vulnerabilities so your software, users, and team stay safe. Join the waitlist to get early access and stay ahead of risks."
  imageSrc="/generated/image-a-cheerful-security-engineer-in-a-cozy-w.webp"
  callsToAction={[
    {
      href: '/waitlist',
      label: 'Join the waitlist',
      variant: 'primary'
    }
  ]}
/>
