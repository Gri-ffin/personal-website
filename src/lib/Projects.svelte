<div id="projects" class="flex flex-col items-center">
	<h3 class="about__heading section-heading">Projects</h3>
	<div class="self-start relative flex mb-[14rem] justify-start">
		<a href="https://classroom-chat-gri-ffin.vercel.app/" target="_blank">
			<div
				class="flex items-center justify-start relative bg-[#3216bb] hover:scale-95 transition-all ease-linear"
			>
				<div class="w-[85%] relative">
					<img src="/classroom.png" alt="Classroom Chat" class="w-full overflow-clip" />
				</div>
			</div>
		</a>
		<div
			class="relative md:top-[3rem] lg:top-[5rem] top-4 h-fit z-50 p-4 -left-[3rem] lg:-left-[5rem] bg-[#1a1a1a80] md:bg-transparent"
		>
			<h3 class="relative z-40 md:text-3xl text-lg font-bold">Classroom Chat</h3>
			<p
				class="relative md:mt-12 mt-1 text-xs md:text-base font-semibold z-50 leading-3 tracking-wider"
			>
				Live chat app for a school project, built using Nextjs, TailwindCss, Firebase.
			</p>
		</div>
	</div>
</div>

<style>
	.section-heading {
		position: relative;
		font-size: 3.5rem;
		font-weight: 700;
		margin-top: 3rem;
		margin-bottom: 3rem;
		z-index: 9999;
	}
	.about__heading:before {
		position: absolute;
		content: '';
		border-bottom: 18px solid #ff4d5a;
		width: 12rem;
		display: block;
		margin: 0 auto;
		position: relative;
		left: 3.5rem;
		top: 4.3rem;
		z-index: -1;
	}
</style>
