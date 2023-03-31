<script lang="ts">
	import ProfileSvg from './svg/ProfileSvg.svelte'

	interface SkillItem {
		label: string
		path: string
	}

	const skillItems: SkillItem[] = [
		{ label: 'Javascript', path: '/js.png' },
		{ label: 'Html', path: '/html.png' },
		{ label: 'Css', path: '/css.png' },
		{ label: 'React', path: '/react.png' },
		{ label: 'Typescript', path: '/ts.svg' },
		{ label: 'Next.Js', path: '/next.png' },
		{ label: 'Node.Js', path: '/node.png' },
		{ label: 'Git', path: '/git.png' },
		{ label: 'Firebase', path: '/firebase.png' }
	]
</script>

<div id="about" class="flex flex-col items-center h-screen">
	<h3 class="about__heading section-heading">About</h3>
	<div
		class="flex flex-col xl:flex-row items-center justify-between w-full md:px-44 px-10 space-y-4"
	>
		<div class="flex items-center flex-col justify-center space-y-4">
			<div class="md:h-44 h-32 flex">
				<ProfileSvg />
			</div>
			<p class="w-full lg:w-[500px] leading-7 tracking-wide text-sm">
				Fully committed to the philosophy of life-long learning, I&apos;m a full stack developer
				with a deep passion for JavaScript, React and all things web development. The unique
				combination of creativity, logic, technology and never running out of new things to
				discover, drives my excitement and passion for web development. When I&apos;m not at my
				computer I like to spend my time reading, playing games or doing some research.
			</p>
		</div>
		<div class="grid gap-4 sm:grid-cols-3 grid-cols-2 h-auto">
			{#each skillItems as skillItem}
				<div class="rounded-md bg-gradient-to-r from-pink-500 via-red-500 to-yellow-500 h-28 p-0.5">
					<div class="h-full flex flex-col items-center p-4 bg-[#1a1a1a]">
						<img class="h-16" src={skillItem.path} alt={skillItem.label} />
						<p class="tracking-wide uppercase">{skillItem.label}</p>
					</div>
				</div>
			{/each}
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
