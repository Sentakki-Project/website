<script setup>
import { onMounted } from 'vue';
import Chart from 'chart.js/auto';

onMounted(() => {
  const ctx = document.getElementById('myChart');
  const myChart = new Chart(ctx, {
    type: 'pie',
    data: {
      labels: ['Bardziej odpowiada mi obecny system', 'Wolał(a)bym używać aplikacji'],
      datasets: [{
        data: [12.5, 87.5,],
        backgroundColor: [
          'rgba(255, 99, 132, 0.2)',
          'rgba(54, 162, 235, 0.2)',
        ],
        borderColor: [
          'rgba(255, 99, 132, 1)',
          'rgba(54, 162, 235, 1)',
        ],
      }]
    },

  });
})

</script>

<template>
  <div>
    <canvas id="myChart" width="400" height="400"></canvas>
  </div>
</template>

<style scoped>

</style>