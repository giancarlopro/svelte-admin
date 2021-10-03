<script>
  import Footer from '../components/organisms/Footer.svelte';
  import Main from '../components/atoms/Main.svelte';
  import Navbar from '../components/organisms/Navbar.svelte';
  import Sidebar from '../components/organisms/Sidebar.svelte';
</script>

<Sidebar />

<Main>
  <Navbar />

  <div class="container-fluid py-4">
    <slot></slot>

    <Footer />
  </div>
</Main>
