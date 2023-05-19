<script >
import AppTitle from './components/AppTitle.vue'
import AppMain from './components/AppMain.vue'
import AppMainComics from './components/AppMainComics.vue'

export default {
  components: {
    AppTitle,
    AppMain,
    AppMainComics,
  }
}
</script>

<template>
  <Header>
    <AppTitle />
  </Header>
  <main>
    <AppMain />
    <AppMainComics />
  </main>
  <footer>

  </footer>
</template>

<style scoped></style>
