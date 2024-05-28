<script lang="ts">
	import '../styles/global.scss';

	import { BookText, Menu } from 'lucide-svelte';
</script>

<div class="h-16 w-lvw bg-blue-900"></div>
<nav
	class="fixed left-[0.5rem] top-2 flex h-12 w-[calc(100vw-1rem)] items-center rounded-lg border-2 border-blue-600 bg-blue-950 bg-opacity-50 text-white backdrop-blur-sm"
>
	<a
		href="https://github.com/typerhextml/typerhext"
		class="size-fit transition hover:text-blue-500 p-2"
	>
		<BookText class="size-6" />
	</a>
	<div class="flex-grow"></div>
	<header class="block h-full pt-1">
		<a
			href="/"
			class="mono block h-full w-fit text-3xl font-black transition hover:text-blue-500"
			>Typer<span class="text-white transition pr-2 ml-1 border-x-white border-x hover:border-x-transparent">Hext</span></a
		>
	</header>
	<div class="flex-grow"></div>
	<label for="menu-open" class="size-fit transition hover:text-blue-500 p-2">
		<Menu class="size-6" />
	</label>
</nav>
<main class="min-h-[calc(100vh-4rem)] bg-blue-900">
	<slot />
</main>
<footer class="bg-blue-950 p-2 text-center text-white">
	&copy; 2024-{new Date().getFullYear()}
	<a
		href="https://leox.dev/"
		class="underline decoration-transparent transition hover:decoration-white">Leonard Lesinski</a
	>
</footer>
