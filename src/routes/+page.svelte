<script>
  import Container from "./Container.svelte";
  import Item from "./Item.svelte";
    import VerticalList from "./VerticalList.svelte";

</script>

<div class="min-h-screen">
  <nav class="p-2">
    <h1 class='font-semibold text-slate-800'>Kanban</h1>
  </nav>
  <main>
    <Container>
      <VerticalList>
        <Item></Item>
        <Item></Item>
        <Item></Item>
        <Item></Item>
        <Item></Item>
      </VerticalList>
      <VerticalList>
        <Item></Item>
        <Item></Item>
        <Item></Item>
        <Item></Item>
        <Item></Item>
      </VerticalList>
      <VerticalList>
        <Item></Item>
        <Item></Item>
        <Item></Item>
        <Item></Item>
        <Item></Item>
      </VerticalList>
    </Container>
  </main>
</div>