<script>
  export let skin = 'default'

  export let label = ''

  import { createEventDispatcher } from 'svelte';

  const dispatch = createEventDispatcher();

  function onClick(event) {
    dispatch('click', event);
  }
</script>

<button
  class="btn btn-{skin}"
  on:click={onClick}>
  {label}
</button>
