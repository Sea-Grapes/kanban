<script>
  import Container from "./Container.svelte";
  import Item from "./Item.svelte";

</script>

<div class="min-h-screen">
  <nav class="p-2">
    <h1 class='font-semibold text-slate-800'>Kanban</h1>
  </nav>
  <main>
    <div class="p-4 bg-slate-100 rounded-md max-w-[40ch]">
      <Container class='space-y-2'>
        <Item></Item>
        <Item></Item>
        <Item></Item>
        <Item></Item>
      </Container>
    </div>
  </main>
</div>