<script setup>
import Item from './Item.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <h1>Oś czasu</h1>
  <Item>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Listopad 2022</template>
    Pomysł projektu i konsultacje z użytkownikami końcowymi.
  </Item>

  <Item>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Grudzień 2022</template>
    Stworzenie architektury aplikacji, dobranie technologii oraz stworzenie makiet w Figmie.
  </Item>

  <Item>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Styczeń - Marzec 2023</template>
    Stworzenie backendu aplikacji w Ruby On Rails oraz integracja z USOS API.
  </Item>

  <Item>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Marzec - Czerwiec 2023</template>
    Stworzenie aplikacji mobilnej w React Native oraz integracja z systemem Stripe.
  </Item>

  <Item>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Czerwiec 2023</template>
    Ostatnie szlify i prezentacja projektu.
  </Item>
</template>
<style scoped>
h1 {
  font-weight: 500;
  font-size: 3.6rem;
  text-align: left;
}


@media (max-width: 767px) {
  h1 {
    font-size: 2.1rem;
  }
}
</style>
