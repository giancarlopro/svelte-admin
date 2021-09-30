<script>
  export let fluid = false
</script>

<div class="container{fluid ? '-fluid' : ''}">
  <slot></slot>
</div>
