<script lang="ts">
	export let name: string, route: string;
	function routing() {
		window.location.href = route;
	}
</script>

<!-- <div>
	{name}
</div> -->

<div class="sidebaritem" on:click={routing}>{name}</div>

<style>
	.sidebaritem {
		display: flex;
		padding: 10px 100px 10px 10px;
		align-items: center;
		gap: 10px;
		flex: 1 0 0;

		color: #598085;
	}
</style>
