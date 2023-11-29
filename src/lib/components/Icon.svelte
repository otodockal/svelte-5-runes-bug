<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children } = $props<{ children?: Snippet }>();
</script>

<span>
	{#if children}
		{@render children()}
	{/if}
</span>
