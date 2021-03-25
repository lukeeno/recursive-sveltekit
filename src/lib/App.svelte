<script>
	import Structure from './Structure.svelte'
	
	const structure = [
		{name: 'foo', component: 'a'},
		{name: 'bar', component: 'b'},
		{name: 'baz', component: 'c', children: [
			{name: 'baz - foo', component: 'a'}
		]}
	]
</script>

<Structure {structure} />