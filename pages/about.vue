<template>
  <section class="hero is-link is-fullheight-with-navbar">
  <div class="hero-body">
    <div class="container">
      <img alt="Hero image" class="hero-background is-transparent" src="@@/assets/img/hero.png" />
      <p class="title">
        Fullheight hero with navbar
      </p>
    </div>
  </div>
</section>
  
</template>

<script>
import Vue from 'vue'
import Buefy from 'buefy'
import 'buefy/dist/buefy.css'
import '@@/assets/css/style.css'

Vue.use(Buefy)

export default {
  head: {
    title: 'About page'
  }
}
</script>