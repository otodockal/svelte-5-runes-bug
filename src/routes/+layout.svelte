<script lang="ts">
	const itemsNav = [
		{
			href: '/',
			title: 'Home',
		},
		{
			href: '/items',
			title: 'Items',
		},
	];
</script>

<nav>
	<ul>
		{#each itemsNav as { href, title }}
			<li>
				<a {href}>
					<span>{title}</span>
				</a>
			</li>
		{/each}
	</ul>
</nav>
<div>
	<slot />
</div>
