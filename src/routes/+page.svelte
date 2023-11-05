<script>
	import '../app.css';

	import Button from '../stories/Button.svelte';
</script>

<h1 class="text-3xl font-bold underline">Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<Button label="clickme">Click me</Button>

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.200);
	}
</style>
