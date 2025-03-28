<script lang='ts'>
  import { onMount } from "svelte";
  let {
    children = null,
    class: className = '',
  } = $props()

  className = className ? `relative ${className}` : 'relative'

  let container: HTMLElement

  onMount(async () => {
    // hacky as jesus
    const Muuri = (await import('muuri')).default

    new Muuri(container, {
      dragEnabled: true
    })
  })

</script>


<div bind:this={container} class={className}>
  {@render children?.()}
</div>