<script setup>
import { onMounted } from 'vue';
import Chart from 'chart.js/auto';

onMounted(() => {
  const ctx = document.getElementById('chartThird');
  const chartThird = new Chart(ctx, {
    type: 'pie',
    data: {
      labels: ['Zdecydowanie się zgadzam', 'Zgadzam się','Nie mam zdania','Nie zgadzam się'],
      datasets: [{
        data: [70,20,5,5],
        backgroundColor: [
          'rgba(126,241,4,0.2)',
          'rgba(54, 162, 235, 0.2)',
          'rgba(243,207,22, 0.2)',
          'rgba(255, 99, 132, 0.2)',

        ],
        borderColor: [
          'rgb(26,241,4,1)',
          'rgba(54, 162, 235, 1)',
          'rgb(243,207,22,1)',
          'rgba(255, 99, 132, 1)',
        ],
      }]
    },

  });
})

</script>

<template>
  <div>
    <canvas id="chartThird" width="400" height="400"></canvas>
  </div>
</template>

<style scoped>

</style>