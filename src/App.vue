<template>
  <div id="app">
    <MainHeader/>
    <MainContent/>
    <MainSidebar/>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainContent from './components/MainContent.vue'
import MainSidebar from './components/MainSidebar.vue'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainSidebar,
  }
}
</script>

<style lang="scss">

  @import './style/index.scss';

</style>