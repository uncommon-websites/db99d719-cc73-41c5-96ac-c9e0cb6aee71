<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";

	// Icons
	import IconFileText from "~icons/lucide/file-text";
	import IconFolderKanban from "~icons/lucide/folder-kanban";
	import IconMessageSquare from "~icons/lucide/message-square";
	import IconSearch from "~icons/lucide/search";
	import IconShieldCheck from "~icons/lucide/shield-check";
	import IconPlug from "~icons/lucide/plug";
</script>

<Hero
	title="Automate your notary workflows and reclaim 3,500 hours annually"
	subtitle="AI-powered document creation, case management, and intelligent communication for German notaries drowning in manual paperwork."
	imageSrc="/generated/image-a-professional-german-notary-in-a-modern.webp"
	centered={false}
	callsToAction={[
		{
			href: "/contact",
			label: "Request demo"
		},
		{
			href: "/about",
			label: "Learn more"
		}
	]}
/>
<LogoScroller 
	label="Trusted by German legal professionals"
	logoUrls={[
		'https://cdn.brandfetch.io/bundesnotarkammer.de/w/400/h/400/logo',
		'https://cdn.brandfetch.io/ra-micro.de/w/400/h/400/logo',
		'https://cdn.brandfetch.io/legartis.ai/w/400/h/400/logo',
		'https://cdn.brandfetch.io/notarnet.de/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="LawX transforms traditional notary offices into efficient, modern practices through AI-powered automation specifically designed for German legal workflows. We eliminate 3,500 hours of manual documentation annually, enabling small and medium-sized notary firms to handle more cases without expanding headcount. Our intelligent platform integrates seamlessly with your existing Microsoft tools, turning administrative burden into competitive advantage while maintaining the highest standards of legal compliance and data security."
/>

<Testimonials
	testimonials={[
		{
			name: "Dr. Klaus Hartmann",
			position: "Notar",
			company: "Kanzlei Hartmann",
			quote:
				"LawX has transformed our practice completely. We now handle 40% more property transactions with the same team size, and document preparation that used to take hours is done in minutes. The AI understands German notary language perfectly.",
			image: "/generated/image-a-professional-german-male-notary-in-a-w.webp"
		},
		{
			name: "Sabine Müller-Weber",
			position: "Notarin",
			company: "Notariat Müller-Weber",
			quote:
				"Before LawX, missed deadlines and manual errors cost us thousands in liability insurance claims. Now our compliance rate is 100%, and we've reduced administrative costs by 30%. The automated case management ensures nothing falls through the cracks.",
			image: "/generated/image-a-professional-german-female-notary-at-h.webp"
		},
		{
			name: "Matthias Schneider",
			position: "Notar",
			company: "Notarbüro Schneider & Partner",
			quote:
				"We were skeptical about AI in legal work, but LawX proved itself immediately. The time saved on document creation alone—over 3,000 hours annually—allowed us to take on 25% more clients without hiring additional staff. The ROI was clear within three months.",
			image: "/generated/image-a-professional-german-male-notary-with-g.webp"
		}
	]}
/>

<Features
	title="Built for the modern notary"
	subtitle="Powerful features that transform how you work"
	features={[
		{
			title: "AI-powered document creation",
			description:
				"Generate legally compliant notary documents in minutes, not hours. Our AI understands German legal requirements and learns from your templates to eliminate repetitive drafting work.",
			icon: IconFileText,
			iconClass: "text-[#006E80]"
		},
		{
			title: "Intelligent case management",
			description:
				"Track every case from intake to completion with automated deadlines and smart reminders. Never miss an obligation or lose track of critical details across multiple matters.",
			icon: IconFolderKanban,
			iconClass: "text-[#0C6E42]"
		},
		{
			title: "Seamless communication hub",
			description:
				"Integrate email, calendar, and messaging into one unified workspace. Connect with clients and partners efficiently while maintaining complete case context at your fingertips.",
			icon: IconMessageSquare,
			iconClass: "text-[#006E80]"
		},
		{
			title: "Semantic document search",
			description:
				"Find any document, clause, or case detail instantly using natural language queries. Advanced AI understands legal context and retrieves exactly what you need in seconds.",
			icon: IconSearch,
			iconClass: "text-[#0C6E42]"
		},
		{
			title: "German legal compliance",
			description:
				"Built on Microsoft Azure with German data residency and strict GDPR compliance. Your client data stays protected with attorney-client privilege safeguards and enterprise security.",
			icon: IconShieldCheck,
			iconClass: "text-[#006E80]"
		},
		{
			title: "Microsoft ecosystem integration",
			description:
				"Works seamlessly with Word, Outlook, and tools you already use daily. Adopt powerful automation without disrupting your established workflows or retraining your team.",
			icon: IconPlug,
			iconClass: "text-[#0C6E42]"
		}
	]}
/>
<AboutTeaser />
<CallToAction 
	title="Join the beta program before September 2025"
	subtitle="Limited spots for forward-thinking notaries"
	description="Be among the first German notaries to automate 3,500 hours of manual work annually. Our September MVP launch is approaching fast, and Design Partner slots are filling quickly. Join practices already saving 30% in costs while handling 20% more cases. Your competitors are already exploring AI—will you lead or follow?"
	imageSrc="/generated/image-a-successful-german-notary-dressed-in-pr.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Request your demo",
			variant: "primary"
		},
		{
			href: "/about",
			label: "Meet the founders",
			variant: "secondary"
		}
	]}
/>
