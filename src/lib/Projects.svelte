<script>
	import LeftSideProject from './Projects/LeftSideProject.svelte'
	import RightSideProject from './Projects/RightSideProject.svelte'
</script>

<svelte:head>
	<link rel="prefetch" href="/classroom.png" />
	<link rel="prefetch" href="/spotify.png" />
	<link rel="prefetch" href="/mangareader.png" />
</svelte:head>

<div id="projects" class="flex flex-col items-center">
	<h3 class="about__heading section-heading">Projects</h3>
	<LeftSideProject
		link="https://classroom-chat-gri-ffin.vercel.app/"
		imageLink="/classroom.png"
		title="Classroom Chat"
		description="Live chat app for a school project, built using Nextjs, TailwindCss, Firebase."
	/>
	<RightSideProject
		link="https://spotify-clone-gri-ffin.vercel.app/login"
		imageLink="/spotify.png"
		title="MySpotify"
		description="Minimal and lightweight Spotify clone that let me listen and enjoy my playlists. Built using Nextjs, TailwindCss, SpotifyApi, Atom."
	/>
	<LeftSideProject
		link="https://manga-reader-gri-ffin.vercel.app/"
		imageLink="/mangareader.png"
		title="Manga Reader"
		description="Website to read japanese manga and the see the latest uploaded manga. Built using Nextjs, ChakraUI, MangadexApi."
	/>
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
