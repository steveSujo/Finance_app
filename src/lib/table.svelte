<script lang="ts">
	export let rows: object[];
	export let columns: string[];
</script>

<table class="table">
	<tr class="tableheader">
		{#each columns as column}
			<th class="columnheading">{column}</th>
		{/each}
	</tr>
	<!-- {#each rows as row}
		<tr class="tablerow">
			<div>{row}</div>
		</tr>
	{/each} -->

	<tr class="tablerow">
		<td>1</td>
		<td>someting</td>
		<td>something more</td>
		<td> #somethign</td>
		<td> /</td>
	</tr>

	<tr class="tablerow">
		<td>2</td>
		<td>someting</td>
		<td>something more</td>
		<td> #somethign</td>
		<td> /</td>
	</tr>
</table>

<style>
	.table {
		border-collapse: collapse;
	}
	.tableheader {
		border-bottom: 1px solid #a3bdc0;
		background: #fff;
		color: #598085;
	}
	.tableheader th:first-child {
		border-radius: 8px 0 0 0;
	}
	.tableheader th:last-child {
		border-radius: 0 8px 0 0;
	}
	.columnheading {
		padding: 0.21rem 0.56rem;

		text-align: left;
		text-transform: uppercase;

		font-style: normal;
		font-weight: 500;
		line-height: normal;
	}

	/* .tableheader :global(p) {
		margin: 0 0.56rem;
	} */

	.tablerow {
		background: #fff;
		color: black;

		border-bottom: 1px solid #a3bdc0;
	}
	.tablerow > td {
		padding: 0.21rem 0.56rem;
	}
	[class~='tablerow']:last-of-type td:last-of-type {
		border-radius: 0 0 8px 0;
	}
	[class~='tablerow']:last-of-type td:first-child {
		border-radius: 0 0 0 8px;
	}
</style>
