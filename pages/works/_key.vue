<template>
  <div class="wrapper">
    <div class="content">
    <!-- {{item}} -->
      <p class="description">{{item.description}}<p>
      <h2 class="title">{{item.title}}</h2>
      <a :href="item.link" class="link" target="_blank">{{item.link}}</a>
      <img :src="item.ui_image">
      <div class="summary">
        <p>{{item.summary}}</p>
        <p>{{item.devenv}}</p>
        <p>{{item.term}}</p>
      </div>
    </div>
  </div>
</template>

<script>
import worklist from '../../components/worklist.js'

export default {
  data () {
    return {
      worklist
    }
  },
  computed: {
    item () {
      return this.worklist[this.$route.params.key]
    }
  }
}
</script>

<style scoped>
.wrapper {
  background-image: url('/contentBg02.png');
  background-repeat: repeat;
  text-align: center;
  padding: 56px 0;
  font-family: "Noto Sans Japanese";
}
.content {
  max-width: 960px;
  margin: 0 auto;
}

img {
  max-width: 100%;
  margin-bottom: 35px;
}

.description {
  font-size: 12px;
  margin-bottom: 7px;
}

.title {
  color: #863461;
  font-size: 32px;
  font-weight: 800;
  margin-bottom: 7px;
}

.link {
  display: block;
  text-decoration: none;
  color: #333;
  font-size: 12px;
  margin-bottom: 35px;
}

.summary {
  width: 40%;
  margin: 0 auto;
  font-size: 14px;
}

.summary p {
  font-weight: 400;
  margin-bottom: 14px;
}
</style>
