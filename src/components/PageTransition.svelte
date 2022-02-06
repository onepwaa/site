<script>
  import { fly } from 'svelte/transition';
  export let refresh = ``;
</script>

{#key refresh}
  <!-- You can modify the in:fly and out:fly attributes to your liking! -->
  <div class="flex flex-grow" in:fly={{ delay: 100, duration: 200, x: -10, }} >
      <slot />
  </div>
{/key}