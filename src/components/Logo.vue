<template>
  <div className="greetings">
    <h1 className="green">{{ displayedMsg }}</h1>
  </div>
</template>

<script setup>
import {ref, onMounted} from 'vue';

const msg = ref('');

msg.value = 'Sentakki Project';

const displayedMsg = ref('');

onMounted(() => {
  let currentIndex = 0;

  const typingInterval = setInterval(() => {
    displayedMsg.value += msg.value[currentIndex];
    currentIndex++;

    if (currentIndex === msg.value.length) {
      clearInterval(typingInterval);
    }
  }, 130);
});
</script>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
  color:#ade5fe;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
