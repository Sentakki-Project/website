<script setup>
import Name from './components/Name.vue';
import History from './components/History.vue';
import Info from "@/components/Info.vue";
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
      <img alt="Vue logo" class="logo" src="./assets/logo.png"/>
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

  </div>
  <div class="scroll-to-top" @click="scrollMain">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-arrow-up">
      <line x1="12" y1="19" x2="12" y2="5"></line>
      <polyline points="5 12 12 5 19 12"></polyline>
    </svg>
  </div>
</template>

<style scoped>
.content{
  display: flex;
  flex-direction: column;
}
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

.full-div {
  top: 0;
  left: 0;
  width: 100%;
  height: 85vh;
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
  .full-div {
    padding: 2rem;
  }
  .time{
    margin-left: 20%;
  }
  .logo {
    max-width: 500px;
  }
}

@media (min-width: 1024px) {
  .full-div {
    padding: 4rem;
  }
}
</style>