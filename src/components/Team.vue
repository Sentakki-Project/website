<template>
  <div class="team-container">
    <h1>Nasz Zespół</h1>
    <div class="person-container">
      <div class="person">
        <img src="/assets/people/raccon.jpg"/>
        <h2>Mikołaj Czurłowski</h2>
        <p>Szop Bakuś</p>
      </div>
      <div class="person">
        <img src="/assets/people/raccon-2.jpg"/>
        <h2>Damian Maza</h2>
        <p>Szop Frontaś</p>
      </div>
      <div class="person">
        <img src="/assets/people/raccon-3.jpg"/>
        <h2>Mateusz Różański</h2>
        <p>Szop Fulstaś</p>
      </div>
      <div class="person">
        <img src="/assets/people/raccon-4.jpg"/>
        <h2>Agnieszka Piszcz</h2>
        <p>Szop Uiksiś</p>
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
  border-radius: 50%;
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
