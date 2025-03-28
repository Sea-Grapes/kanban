<script lang="ts">
	import '../app.css';
	
	let { children } = $props();
</script>

<svelte:head>
  <title>Kanban</title>
</svelte:head>

{@render children()}
