<script lang="ts">
	import { onMount } from 'svelte'
	import { fly } from 'svelte/transition'
	let visible: boolean = false

	onMount(() => {
		visible = true
	})
</script>

<div
	class="flex flex-col items-center justify-center h-screen tracking-widest text-center space-y-2"
>
	{#if visible}
		<p transition:fly={{ x: 50, duration: 2000 }} class="text-2xl md:text-4xl">
			Hello, I&apos;m <span class="text-[#ff4d5a]">Yassine</span>
		</p>
		<p transition:fly={{ x: -50, duration: 2000 }} class="text-2xl md:text-4xl">
			I&apos;m a full stack web developer.
		</p>
		<button
			transition:fly={{ y: 50, delay: 2000, duration: 2000 }}
			class="outline p-2 outline-[#ff4d5a] text-[#ff4d5a] hover:outline-[#ec2c39ab]"
			>View my projects</button
		>
	{/if}
</div>
