<script>
  import { slide } from 'svelte/transition';

  export let key;
  export let duration = 300;
</script>

{#key key}
  <div class="gradient h-full"
    in:slide={{ duration: 0, y: -100 }}
    out:slide={{ duration, y: 100 }}
  >
    <slot />
  </div>
{/key}

<style>
  div {
    display: grid;
    place-content: center;
  }
</style>
