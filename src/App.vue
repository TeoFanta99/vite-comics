<script >
import AppHeader from './components/AppHeader.vue'
import ListProducts from './components/ListProducts.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    ListProducts,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <ListProducts />
  </main>
  <footer>
    <AppFooter />
  </footer>
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
