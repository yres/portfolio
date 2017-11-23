<template>
  <section class="container">
    <header class="headline">
      <h1 class="title">yres_matome</h1>
      <p class="name">Portfolio of yajima yurie.</p>
    </header>
    <Profile />
    <Skills />
    <Works />
    <Social />
  </section>
</template>

<script>
import Profile from '../components/Profile.vue'
import Skills from '../components/Skills.vue'
import Works from '../components/Works.vue'
import Social from '../components/Social.vue'

export default {
  data () {
    return {
      title: 'yres_memo!'
    }
  },
  head () {
    return {
      title: 'yres_memo!'
    }
  },
  components: {
    Profile,
    Skills,
    Works,
    Social
  }
}
</script>

<style lang="scss" scoped>
.container {
  text-align: center;
  font-family: "Noto Sans Japanese";
}
.headline {
  width: 100%;
  display: block;
  background-image: url('../static/header.png');
  color: #fff;
  padding: 65px 0;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 48px;
  letter-spacing: 1px;
  padding-bottom: 14px;
}
.name {
  margin-bottom: 35px;
}

</style>
