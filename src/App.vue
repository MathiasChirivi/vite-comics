<script >
import AppTitle from './components/AppTitle.vue'
import AppMain from './components/AppMain.vue'
import AppMainSeries from './components/AppMainSeries.vue'
import AppMainComics from './components/AppMainComics.vue'
import AppFooterImg from './components/AppFooterImg.vue'
import AppFooterFollow from './components/AppFooterFollow.vue'

import comicsDataJson from './data/comics.json'


export default {
  components: {
    AppTitle,
    AppMain,
    AppMainSeries,
    AppMainComics,
    AppFooterImg,
    AppFooterFollow
  },
  data() {
    return {
      itemsComicListJson: comicsDataJson,
    }
  }
}
</script>

<template>
  <Header>
    <AppTitle />
  </Header>
  <main>
    <AppMain />
    <AppMainSeries :itemsComic="itemsComicListJson" />
    <AppMainComics />
  </main>
  <footer>
    <AppFooterImg />
    <AppFooterFollow />
  </footer>
</template>

<style scoped></style>
