<template>
  <div id="app">
    <AppHeader />
    <main>
      <router-view></router-view>
    </main>
    <AppFooter />
   </div>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue'
import AppFooter from '@/components/AppFooter.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<style lang="less">
* {
  padding: 0;
  margin: 0;
  border: 0;
  box-sizing: border-box;
}
#app {
  font-family: sans-serif;
  background: #f5f5f5;
  overflow-x: hidden;
}
main {
  height: calc(100vh - 16vh);
   /*
  padding: 0 6vw 0 6vw;
  display: flex;
  justify-content: center;
  margin: 3%; */
}
</style>