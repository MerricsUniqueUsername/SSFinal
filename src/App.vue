<template>
  <Navbar @changePage="changePage" />

  <Home v-if="page === 'home'" />
  <FAQ v-if="page === 'faq'" />
  <Sources v-if="page ==='sources'" />
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import FAQ from './components/FAQ.vue'
import Sources from './components/Sources.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    FAQ,
    Sources,
  },
  data() {
    return {
      page: 'home',
    }
  },
  methods: {
    changePage(page) {
      this.page = page;
    }
  }

}
</script>

<style>

</style>