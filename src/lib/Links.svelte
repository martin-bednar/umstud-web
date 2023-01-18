<script>
	const links = [
		{ href: '/press', label: 'Press' },
		{ href: '/about', label: 'About' }
	];
</script>

<ul
	id="links"
	class="
	m-0 
	mr-2 
	flex 
	h-full 
	list-none 
	items-center 
	justify-start 
	divide-x
	p-0"
>
	{#each links as link}
		<li class="flex h-full w-40 items-center justify-center pl-2 pr-2">
			<a
				href={link.href}
				class="
				flex 
				h-16 w-16 
				items-center justify-center 
				rounded-full border border-black 
				text-center uppercase text-inherit no-underline 
				transition-colors duration-500 
				hover:bg-black hover:text-white"
			>
				<span>{link.label}</span>
			</a>
		</li>
	{/each}
</ul>
