<script>
	import A from './A.svelte'
	import B from './B.svelte'
	import C from './C.svelte'
	
	export let structure
	
	const componentMap = {
		a: A,
		b: B,
		c: C
	}
</script>

{#each structure as block}
	<svelte:component this={componentMap[block.component]} {block} />
{/each}