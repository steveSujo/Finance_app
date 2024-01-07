<script lang="ts">
	import Sidebaritem from './sidebaritem.svelte';
</script>

<div class="sidebar">
	<p>sidebar::comp</p>
	<div class="items">
		<Sidebaritem name="Dashboard" route="/app/dashboard/" />
		<Sidebaritem name="Inventory" route="/app/inventory/" />
		<Sidebaritem name="Invoices" route="/app/invoices/" />
		<Sidebaritem name="Account" route="/app/accounts/" />
		<Sidebaritem name="Report" route="/app/report/" />
	</div>
	<Sidebaritem name="Settings" route="/app/settings/" />
</div>

<style>
	.sidebar {
		display: flex;
		width: 16.66667rem;
		height: 50.22222rem;
		padding: 0.55556rem 1.77778rem;
		flex-direction: column;
		align-items: flex-start;
		gap: 4rem;
		flex-shrink: 0;

		border-right: 1px solid rgba(89, 128, 133, 0.69);
		background: #f9fafb;
	}
	.items {
		display: flex;
		padding: 10px 0px;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
		gap: 8px;
		align-self: stretch;
	}
</style>
