<script setup>
import { onMounted } from 'vue';
import Chart from 'chart.js/auto';



onMounted(() => {
  const ctx = document.getElementById('chartFirst');
  const chartFirst = new Chart(ctx, {
    type: 'pie',
    data: {
      labels: ['Zdecydowanie się zgadzam', 'Zgadzam się','Nie mam zdania'],
      datasets: [{
        data: [80,15,5],
        backgroundColor: [
          'rgba(126,241,4,0.2)',
          'rgba(54, 162, 235, 0.2)',
          'rgb(243,207,22,0.2)',

        ],
        borderColor: [
          'rgb(126,241,4,1)',
          'rgba(54, 162, 235, 1)',
          'rgb(243,207,22,1)',
        ],
      }]
    },

  });
})

</script>

<template>
  <div>
    <canvas id="chartFirst" width="400" height="400"></canvas>
  </div>
</template>

<style scoped>

</style>