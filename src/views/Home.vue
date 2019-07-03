<template>
  <div class="home">
    <Top />
    <Search />
    <Login />
    <Footer></Footer>
  </div>
</template>

<script>
// @ is an alias to /src
import Top from '@/components/Header/top.vue'
import Search from '@/components/Header/search.vue'
import Footer from '@/components/Footer/footer.vue'
import Login from '@/views/Login/login.vue'

export default {
  name: 'home',
  components: {
    Top, Search, Login, Footer
  }
}
</script>
