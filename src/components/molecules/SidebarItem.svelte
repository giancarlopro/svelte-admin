<script>
  export let href = ''
  export let label = ''
  export let active = false
</script>

<style>
  a.active > div.icon > :global(i) {
    color: white !important;
  }

  a > div.icon > :global(i) {
    color: black !important;
  }
</style>

<li class="nav-item">
  <a class="nav-link {active ? 'active': ''}" href="{href}">
    <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
      <slot></slot>
    </div>
    <span class="nav-link-text ms-1">{label}</span>
  </a>
</li>
