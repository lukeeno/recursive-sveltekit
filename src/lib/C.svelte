<script>
	import Structure from './Structure.svelte'
	
	export let block
</script>

<Structure structure={block.children} />