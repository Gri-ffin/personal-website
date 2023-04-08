<script lang="ts">
	import About from '$lib/About.svelte'
	import Contact from '$lib/Contact.svelte'
	import Nav from '$lib/Nav.svelte'
	import Projects from '$lib/Projects.svelte'
	import Welcome from '$lib/Welcome.svelte'
	import './styles.css'
</script>

<main class="text-[#fafafa]">
	<Nav />
	<Welcome />
	<About />
	<Projects />
	<Contact />
</main>
