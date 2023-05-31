<script setup>

</script>

<template>
  <div class="info-container">
    <h1>Czym jest projekt Sentakki?</h1>
    <p>
      Nazwa Sentakki wywodzi się z języka japońskiego (洗濯機) i oznacza pralnie lub pralnie.
      Naszym głównym celem jest ułatwienie codziennego życia studentów i personelu akademickiego
      poprzez dostarczanie efektywnych narzędzi do zarządzania pralniami w akademikach.
      Nasza aplikacja Sentakki umożliwia studentom łatwe rezerwowanie pralni w dogodnym dla nich czasie. Dzięki niej użytkownicy mogą sprawdzić dostępność pralek.
      Jedną z głównych zalet naszej aplikacji jest możliwość płatności online. Użytkownicy mogą dokonywać płatności za pranie bezpośrednio z aplikacji.
    </p>
  </div>
</template>

<style scoped>
.info-container{
  width:100%;
}
p{
  font-size: 1.5rem;
}
h1{
  font-weight: 500;
  font-size: 3.6rem;
}
@media (max-width: 767px) {
  h1 {
    font-size: 2.1rem;
  }
  p{
    font-size: 1rem;
  }
}
</style>
