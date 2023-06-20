<script setup>
import Name from './components/Name.vue';
import History from './components/History.vue';
import Info from "@/components/Info.vue";
import Stack from "@/components/Stack.vue";
import Chart from "@/components/Chart.vue";
import ChartDescription from "@/components/ChartDescription.vue";
import Team from "@/components/Team.vue";
import ChartFirst from "@/components/ChartFirst.vue";
import ChartDescriptionFirst from "@/components/ChartDescriptionFirst.vue";
import CharDescriptionSecond from "@/components/ChartDescriptionSecond.vue";
import ChartSecond from "@/components/ChartSecond.vue";
import ChartThird from "@/components/ChartThird.vue";
import ChartDescriptionThird from "@/components/ChartDescriptionThird.vue";
import ChartDescriptionFourth from "@/components/ChartDescriptionFourth.vue";
import ChartFourth from "@/components/ChartFourth.vue";
import Plans from "@/components/Plans.vue";
const scrollMain = () => {
  const mainSection = document.getElementById('start');
  if (mainSection) {
    mainSection.scrollIntoView({ behavior: 'smooth' });
  }
}
</script>

<template>
  <div class="content">
    <div class="full-div" id="start">
      <img alt="logo" class="logo" src="../public/assets/logo.png"/>
      <div class="wrapper">
        <Name/>
      </div>
    </div>
    <div class="full-div">
      <Info/>
    </div>
    <div class="full-div time">
      <History/>
    </div>
    <div class="chart-container">
      <div class="chart-description">
        <ChartDescription />
      </div>
      <div class="chart">
        <Chart />
      </div>
    </div>
    <div class="chart-container">
      <div class="chart-description">
        <ChartDescriptionFirst />
      </div>
      <div class="chart">
        <ChartFirst />
      </div>
    </div>
    <div class="chart-container">
      <div class="chart-description">
        <CharDescriptionSecond />
      </div>
      <div class="chart">
        <ChartSecond />
      </div>
    </div>
    <div class="chart-container">
      <div class="chart-description">
        <ChartDescriptionThird />
      </div>
      <div class="chart">
        <ChartThird />
      </div>
    </div>
    <div class="chart-container">
      <div class="chart-description">
        <ChartDescriptionFourth />
      </div>
      <div class="chart">
        <ChartFourth />
      </div>
    </div>
    <div class="full-div">
      <Plans/>
    </div>
    <div class="full-div">
      <Stack/>
    </div>
    <div class="full-div">
      <Team/>
    </div>
  </div>
  <div class="scroll-to-top" @click="scrollMain">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-arrow-up">
      <line x1="12" y1="19" x2="12" y2="5"></line>
      <polyline points="5 12 12 5 19 12"></polyline>
    </svg>
  </div>
</template>

<style scoped>

.scroll-to-top {
  position: fixed;
  bottom: 2rem;
  right: 2rem;
  width: 40px;
  height: 40px;
  background-color: #000;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

.scroll-to-top svg {
  width: 20px;
  height: 20px;
  fill: currentColor;
}
.content{
  display: flex;
  flex-direction: column;
}
.chart-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  justify-content: center;
  padding: 2rem;
  box-sizing: border-box;
}

.chart-description {
  margin-bottom: 1rem;
}
.full-div {
  top: 0;
  left: 0;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 2rem;
  box-sizing: border-box;
}
.time{
  align-items: stretch;
}

.logo {
  width: 100%;
  max-width: 300px;
  margin-bottom: 2rem;
}

@media (min-width: 768px) {
  #header {
    font-size: 2.1rem;
  }
  .full-div {
    padding: 2rem;
    height: 85vh;
  }

  .time{
    margin-left: 20%;
  }
  .logo {
    max-width: 500px;
  }
  .chart-container {
    height: 85vh;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
  .chart-description {
    margin-bottom: 0;
    margin-right: 2rem;
  }
}

@media (min-width: 1024px) {
  .full-div {
    padding: 4rem;
  }
}
</style>
