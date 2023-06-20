<template>
  <div class="team-container">
    <h1>Nasz Zespół</h1>
    <div class="person-container">
      <div class="person">
        <img src="../../public/assets/people/racoon.png"/>
        <h2>Mikołaj Czurłowski</h2>
        <p>Backend Developer</p>
      </div>
      <div class="person">
        <img src="../../public/assets/people/racoon-3.png"/>
        <h2>Damian Maza</h2>
        <p>Frontend Developer</p>
      </div>
      <div class="person">
        <img src="../../public/assets/people/racoon-2.png"/>
        <h2>Mateusz Różański</h2>
        <p>Fullstack Developer</p>
      </div>
      <div class="person">
        <img src="../../public/assets/people/racoon-1.png"/>
        <h2>Agnieszka Piszcz</h2>
        <p>UI/UX Developer</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
h2 {
  font-weight: 600;
}
p {
  font-weight: 500;
  text-align: center;
}
.team-container {
  display: flex;
  flex-direction: column;
  align-items: center; /* Wyśrodkowanie na osi poziomej */
  justify-content: center; /* Wyśrodkowanie na osi pionowej */
  text-align: center;
}

.person-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center; /* Wyśrodkowanie elementów na osi poziomej */
}

.person {
  flex-basis: 50%;
  padding: 1rem;
  box-sizing: border-box;
  text-align: center;
}

@media (min-width: 768px) {
  .person {
    flex-basis: 25%;
  }
}

img {
  width: 200px;
  height: 200px;
}

h1 {
  font-weight: 500;
  font-size: 3.6rem;
  margin-bottom: 1rem;
}

@media (max-width: 767px) {
  h1 {
    font-size: 2.1rem;
  }
}
</style>
