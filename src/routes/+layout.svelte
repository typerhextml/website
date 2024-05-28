<script lang="ts">
	import '../styles/global.scss';

  import { BookText, Menu } from 'lucide-svelte';
</script>

<div class="h-16 w-lvw bg-blue-900"></div>
<nav
	class="fixed left-[0.5rem] top-2 h-12 w-[calc(100vw-1rem)] rounded-lg border-2 border-blue-600 bg-blue-950 bg-opacity-50 text-white backdrop-blur-sm flex p-2 items-center"
>
  <a href="https://github.com/typerhextml/typerhext" class="size-fit hover:text-blue-500 transition">
    <BookText class="size-6" />
  </a>
  <div class="flex-grow"></div>
	<header>
		<a href="/" class="mono text-3xl font-black h-fit w-fit block pb-1">TyperHext</a>
	</header>
  <div class="flex-grow"></div>
  <label for="menu-open" class="size-fit hover:text-blue-500 transition">
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
