<script lang="ts">
	import FaGithub from 'svelte-icons/fa/FaGithub.svelte'
	import FaLinkedin from 'svelte-icons/fa/FaLinkedin.svelte'
	import IoIosMail from 'svelte-icons/io/IoIosMail.svelte'

	const thisYear = new Date().getFullYear()
</script>

<footer class="bg-[#282828f2] flex flex-col items-center justify-center py-5">
	<div class="flex gap-4">
		<a href="https://github.com/gri-ffin" class="w-7 h-7 hover:text-redrose scale-125">
			<FaGithub />
		</a>
		<a href="https://linkedin.com/in/yassine-tadlaoui" class="w-7 h-7 hover:text-redrose scale-125">
			<FaLinkedin />
		</a>
		<a href="mailto:yassinetadlaoui8@gmail.com" class="w-8 h-8 hover:text-redrose scale-125">
			<IoIosMail />
		</a>
	</div>
	<p>Yassine Tadlaoui &copy; {thisYear}</p>
</footer>
