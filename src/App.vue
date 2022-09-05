<template>
  <div id="app">
    <MainHeader/>
    <MainContent/>
    <MainSidebar/>
    <MainFooter/>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainContent from './components/MainContent.vue'
import MainSidebar from './components/MainSidebar.vue'
import MainFooter from './components/MainFooter.vue'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainSidebar,
    MainFooter,
  }
}
</script>

<style lang="scss">

  @import './style/index.scss';

</style>