<template>
  <div id="app">
    <Top />
    <Search />
    <Navbar></Navbar>
    <router-view />
    <Footer></Footer>
  </div>
</template>

<script>
import Top from '@/components/Header/top.vue'
import Search from '@/components/Header/search.vue'
import Footer from '@/components/Footer/footer.vue'
import Login from '@/views/Login/login.vue'
import Navbar from '@/components/Navbar/navbar.vue'
export default {
  name: 'App',
  components: {
    Top, Search, Login, Footer, Navbar
  }
}
</script>


<style lang="less">
@import url("../src/assets/base.less");
@import url("../src/assets/normalize.css");
@import url("./assets/font-awesome.css");

#app {
  font-family: "Microsoft YaHei", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #464459;
}
.inner {
  margin: 0 auto;
  width: @base-width;
}
</style>
