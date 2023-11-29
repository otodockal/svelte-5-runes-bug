# svelte-5-runes-bug

### Describe the bug

On route navigation in SvelteKit (together with Svelte 5 runes), I encountered the error `Cannot read null properties (reads 'isConnected')`. There might be a bug related to **snippet_effect** or **create_snippet_block** fns...At some point block.d becomes [null] for some reason.

### Reproduction

Click on the link "Items" and the content is not rendered. Open console.

- svelte 5.0.0-next.15
- @sveltejs/kit 1.27.6.

### Refs

- Issue: https://github.com/sveltejs/svelte/issues/9678
- PR: https://github.com/sveltejs/svelte/pull/9675