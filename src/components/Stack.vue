<template>
  <h1>Jakie technologie wykorzystaliśmy?</h1>
  <div className="technologies">
    <img src="../../public/assets/technology/ror-logo.png" alt="Ruby on Rails logo"/>
    <img src="../../public/assets/technology/react-native-logo.png" alt="React native logo"/>
    <img src="../../public/assets/technology/vue-logo.png" alt="Vue logo"/>
    <img src="../../public/assets/technology/docker-logo.png" alt="Docker logo"/>
    <img src="../../public/assets/technology/figma-logo.png" alt="Figma logo"/>
    <img src="../../public/assets/technology/heroku-logo.png" alt="Heroku logo"/>
    <img src="../../public/assets/technology/firebase-logo.png" alt="Firebase logo"/>
    <img src="../../public/assets/technology/postgresql-logo.png" alt="Posgresql logo"/>
  </div>

</template>

<style scoped>
h1{
  font-weight: 500;
  font-size: 3.6rem;
  margin-bottom: 1.4rem;
}
.technologies {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 50px;
}

.technologies img {
  width: 150px;
  height: 150px;
}

@media (max-width: 767px) {
  .technologies {
    grid-template-columns: 1fr;
  }
  h1 {
    font-size: 2.1rem;
  }
  .technologies img {
    width: 100px;
    height: 100px;
  }
}
</style>
<script setup>
</script>