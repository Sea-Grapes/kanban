<script lang='ts'>
  import { onMount } from "svelte";
  let { children = null } = $props()

  let container: HTMLElement

  onMount(async () => {
    // hacky as jesus
    const Muuri = (await import('muuri')).default

    new Muuri(container, {
      dragEnabled: true
    })
  })

</script>

<div class='p-4 bg-slate-100 rounded-md max-w-[40ch]'>
  <div bind:this={container} class='relative space-y-2'>
    {@render children?.()}
  </div>
</div>