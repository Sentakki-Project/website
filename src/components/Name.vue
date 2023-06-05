<template>
  <div className="greetings">
    <h1 className="green">{{ displayedMsg }}</h1>
  </div>
</template>

<script setup>
import {ref, onMounted} from 'vue';

const msg = ref('...');

msg.value = 'entakki Project';

const displayedMsg = ref('S');
const startTypingAnimation = () => {
  let currentIndex = 0;
  const typingInterval = setInterval(() => {
    displayedMsg.value += msg.value[currentIndex];
    currentIndex++;

    if (currentIndex === msg.value.length) {
      clearInterval(typingInterval);
      setTimeout(() => {
        displayedMsg.value = 'S';
        startTypingAnimation();
      }, 4500);
    }
  }, 130);
};
onMounted(() => {
  startTypingAnimation();
});
</script>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 3.6rem;
  top: -10px;
  color:#ade5fe;
}


.greetings h1 {
  text-align: center;
}
@media (prefers-color-scheme: light){
  h1{
    color:#555555;
  }
}
@media (max-width: 767px) {
  h1 {
    font-size: 2.1rem;
  }
}
</style>
