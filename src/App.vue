<script >
import AppHeader from './components/AppHeader.vue'
import ListProducts from './components/ListProducts.vue'

export default {
  components: {
    AppHeader,
    ListProducts
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <ListProducts />
  </main>
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $primary;
}
</style>
