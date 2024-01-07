<script lang="ts">
	import Sidebar from '$lib/sidebar.svelte';
</script>

<Sidebar />
<div class="fulls">
	<slot />
</div>

<style>
	div {
		padding: 0 0.5rem;
		/* padding-top: 0.5rem; */
		background: #f5f5f5;
	}
</style>
