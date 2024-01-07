<script lang="ts">
	import Table from '$lib/table.svelte';
	let rows: object[] = [
		{ id: 1, desc: 'somthing1' },
		{ id: 1, desc: 'somthing1' },
		{ id: 1, desc: 'somthing1' }
	];
	let columns = ['id', 'title', 'desc', 'tag', 'url'];
</script>

<div>
	<p>Accounts: page data :test</p>
	<Table {rows} {columns}></Table>
</div>

<style>
	div {
		color: blue;
	}
</style>
