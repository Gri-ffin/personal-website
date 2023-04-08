<script lang="ts">
	export let link: string
	export let imageLink: string
	export let title: string
	export let description: string
</script>

<div class="self-start relative flex md:mb-[14rem] mb-[6rem] justify-start">
	<a href={link} target="_blank">
		<div
			class="flex items-center justify-start relative bg-[#3216bb] hover:scale-95 transition-all ease-linear"
		>
			<div class="w-[85%] relative">
				<img src={imageLink} alt={title} class="w-full overflow-clip" />
			</div>
		</div>
	</a>
	<div
		class="relative md:top-[3rem] lg:top-[5rem] top-4 h-fit z-40 p-4 -left-[3rem] lg:-left-[5rem] bg-[#1a1a1a80] md:bg-transparent"
	>
		<h3 class="relative z-40 md:text-3xl text-lg font-bold">{title}</h3>
		<p
			class="relative md:mt-8 mt-1 md:mb-6 mb-1 text-xs md:text-base font-semibold z-50 leading-3 tracking-wider"
		>
			{description}
		</p>
		<a
			href={link}
			target="_blank"
			class="font-semibold tracking-wider relative underline-animation text-sm md:text-xl"
			>Live app</a
		>
	</div>
</div>

<style>
	@keyframes underline {
		0% {
			width: 100%;
			right: 0;
		}
		100% {
			width: 0;
			right: 100%;
		}
	}

	.underline-animation::before {
		content: '';
		position: absolute;
		left: 0;
		bottom: 0;
		width: 100%;
		height: 2px;
		background-color: #ff4d5a;
		transition: width 0.5s ease-out;
		text-underline-offset: 8px;
	}

	.underline-animation:hover::before {
		animation: underline 0.5s ease-out forwards;
		overflow: hidden;
	}
</style>
