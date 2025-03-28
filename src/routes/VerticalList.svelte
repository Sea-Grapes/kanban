<script>
  import Container from "./Container.svelte";
  let { children } = $props()
</script>

<div class="absolute p-4 pb-2 bg-slate-100 rounded-md w-[40ch] mr-4 space-y-8">
  <h1 class="text-2xl font-bold">Header</h1>
  <Container>
    {@render children?.()}
  </Container>
</div>