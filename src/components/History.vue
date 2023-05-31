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
    Pomysł Projektu
  </Item>

  <Item>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Grudzień 2022</template>
    Stworzenie Architektury Aplikacji, dobranie technologii oraz stworzenie makiet w Figmie
  </Item>

  <Item>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Styczeń - Marzec 2023</template>
    Stworzenie backendu aplikacji w Ruby On Rails
  </Item>

  <Item>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Marzec - Czerwiec 2023</template>
    Stworzenie aplikacji mobilnej w React Native
  </Item>

  <Item>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Czerwiec 2023</template>
    Prezentacja projektu
  </Item>
</template>
<style scoped>
h1 {
  font-weight: 500;
  font-size: 3.6rem;
}


@media (max-width: 767px) {
  h1 {
    font-size: 2.1rem;
  }
}
</style>
