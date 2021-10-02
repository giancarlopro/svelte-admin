<script>
  import Chart from 'chart.js/auto';

	import { onMount } from 'svelte';

	let chartValues = [1, 2, 3, 4, 5, 6, 7];
	let chartLabels = ['Doming', 'Segunda', 'Terça', 'Quarta', 'Quinta', 'Sexta', 'Sábado'];
	let ctx;
	let chartCanvas;

	onMount(async (promise) => {
    ctx = chartCanvas.getContext('2d');
    var chart = new Chart(ctx, {
      type: 'bar',
      data: {
        labels: chartLabels,
        datasets: [{
          label: 'Passagens',
          backgroundColor: '#cb0c9f',
          borderColor: '#cb0c9f',
          data: chartValues
        }]
      }
		});
	});
</script>

<div class="col-lg-7 mt-4">
  <div class="card z-index-2">
    <div class="card-header pb-0">
      <h6>Passagens na semana</h6>
      <!-- <p class="text-sm">
        <i class="fa fa-arrow-up text-success"></i>
        <span class="font-weight-bold">4% more</span> in 2021
      </p> -->
    </div>
    <div class="card-body p-3">
      <div class="chart">
        <canvas bind:this={chartCanvas} id="chart-line" class="chart-canvas"></canvas>
      </div>
    </div>
  </div>
</div>