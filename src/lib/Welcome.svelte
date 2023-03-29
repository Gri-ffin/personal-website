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
			Hello, I&apos;m <span class="text-redrose">Yassine</span>
		</p>
		<p transition:fly={{ x: -50, duration: 2000 }} class="text-2xl md:text-4xl">
			I&apos;m a full stack web developer.
		</p>
		<button
			transition:fly={{ y: 50, delay: 2000, duration: 2000 }}
			class="outline p-2 outline-redrose text-redrose hover:outline-[#ec2c39ab] space-x-2 text-sm md:text-base"
			>View my projects <svg
				class="rotate-90 fill-redrose inline-block"
				version="1.1"
				xmlns="http://www.w3.org/2000/svg"
				width="24"
				height="24"
				viewBox="0 0 24 24"
				><title>arrow-right</title><path
					d="M11.293 5.707l5.293 5.293h-11.586c-0.552 0-1 0.448-1 1s0.448 1 1 1h11.586l-5.293 5.293c-0.391 0.391-0.391 1.024 0 1.414s1.024 0.391 1.414 0l7-7c0.092-0.092 0.166-0.202 0.217-0.324 0.101-0.245 0.101-0.521 0-0.766-0.049-0.118-0.121-0.228-0.217-0.324l-7-7c-0.391-0.391-1.024-0.391-1.414 0s-0.391 1.024 0 1.414z"
				/></svg
			>
		</button>
	{/if}
</div>
