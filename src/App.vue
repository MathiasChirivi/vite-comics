<script >
import AppTitle from './components/AppTitle.vue'
import AppMain from './components/AppMain.vue'
import AppMainComics from './components/AppMainComics.vue'
import AppFooterImg from './components/AppFooterImg.vue'


export default {
  components: {
    AppTitle,
    AppMain,
    AppMainComics,
    AppFooterImg,
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
    <AppFooterImg />
  </footer>
</template>

<style scoped></style>
