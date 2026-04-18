<script lang="ts">
	import {
		faBluesky,
		faDiscord,
		faGithub,
		faInstagram,
		faTwitter,
		faYoutube,
	} from '@fortawesome/free-brands-svg-icons';
	import { icon, type IconDefinition } from '@fortawesome/fontawesome-svg-core';
	import Logo from '$lib/assets/logo.png';
	import Lobby from '$lib/assets/lobby.png';
</script>

{#snippet Social(iconDefinition: IconDefinition, url: string)}
	<a href={url} class="transition-all hover:scale-110 hover:text-amber-50">
		{@html icon(iconDefinition).html}
	</a>
{/snippet}

<section
	class="flex h-screen w-screen flex-col items-center justify-center gap-2 overflow-scroll bg-[#20030a] p-16 text-center text-[#8F5921] *:z-10"
>
	<img
		src={Lobby}
		aria-hidden={true}
		alt="Hellscape"
		class="fixed z-0 h-full w-full scale-120 object-cover object-center opacity-50 blur-xs brightness-20 select-none"
	/>
	<img src={Logo} alt="Welcome To Hell Logo" class="mb-4 w-96" />
	<h1 class="relative z-10 w-full text-center text-5xl leading-11 font-bold text-amber-50">
		Chapter 1
		<!-- wtf lmao -->
		<i
			class="absolute top-0 left-0 -z-10 inline-flex h-full w-full items-center justify-center text-6xl font-light tracking-widest text-[#8F5921] opacity-50"
			>A Star Upon A Child</i
		>
		<br />
		<span class="mr-px">December 2026</span>
	</h1>
	<p class="max-w-[60ch] text-sm text-balance">
		<span class="font-semibold">Welcome To Hell</span> is an experimental tower-obby game with inventive gameplay expanding
		on true-to-its-roots inspirations, all woven together with a rewarding narrative, set in an incinerated Caelum.
	</p>
	<div class="mt-2 flex items-center justify-center gap-1">
		{@render Social(faDiscord, 'https://discord.gg/9Fuv68NcSt')}
		{@render Social(faYoutube, 'https://www.youtube.com/@welcomestohell')}
		{@render Social(faInstagram, 'https://www.instagram.com/welcomestohell/')}
		{@render Social(faBluesky, 'https://bsky.app/profile/welcomestohell.com')}
		{@render Social(faTwitter, 'https://x.com/welcomestohell')}
		{@render Social(faGithub, 'https://github.com/welcomestohell')}
	</div>
</section>
