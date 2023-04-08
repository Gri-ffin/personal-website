<script lang="ts">
	import { page } from '$app/stores'
</script>

<nav
	class="fixed bg-[#282828f2] flex justify-center md:justify-end items-center md:h-14 border-b backdrop-filter z-50 shadow-lg border-black w-full text-sm h-10 md:text-base"
>
	<ul class="flex md:mr-12 md:gap-10 gap-5">
		<li>
			<a
				href="#welcome"
				class={`${$page.url.hash === '#welcome' || $page.url.hash === '' ? 'text-redrose' : ''}`}
				>Home</a
			>
		</li>
		<li>
			<a href="#about" class={`${$page.url.hash === '#about' ? 'text-redrose' : ''}`}>About</a>
		</li>
		<li>
			<a href="#projects" class={`${$page.url.hash === '#projects' ? 'text-redrose' : ''}`}
				>Projects</a
			>
		</li>
	</ul>
</nav>
