<script>
import Main from '../atoms/Main.svelte';
import DailyReport from '../organisms/dashboard/DailyReport.svelte';
import ResumeCards from '../organisms/dashboard/ResumeCards.svelte';
import WeeklyReport from '../organisms/dashboard/WeeklyReport.svelte';
import Navbar from '../organisms/Navbar.svelte';
import Sidebar from '../organisms/Sidebar.svelte';
</script>

<Sidebar />
<Main>
  <Navbar title="Dashboard" />

  <div class="container-fluid py-4">
    <ResumeCards />

    <div class="row mt-4">
      <WeeklyReport />
      <DailyReport />
    </div>
  </div>
</Main>
