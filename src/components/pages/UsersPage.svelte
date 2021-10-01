<script>
import Main from '../atoms/Main.svelte';
import Navbar from '../organisms/Navbar.svelte';

import Sidebar from '../organisms/Sidebar.svelte';
import UsersTable from '../organisms/users/UsersTable.svelte';
</script>

<Sidebar active='usuarios' />
<Main>
  <Navbar title="Usuáros" />

  <UsersTable />
</Main>
