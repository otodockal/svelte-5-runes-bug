<script lang="ts">
	let { data } = $props<{ data: { items: { title: string }[] } }>();
</script>

{#each data.items as item}
	<div>
		{item.title}
	</div>
{/each}
