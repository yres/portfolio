<template>
  <section>
    <h2 class="title">WORKS</h2>
    <ul>
      <li v-for="(item, key) in list" :key="key">
        <nuxt-link :to="{path: `works/${key}`}" class="link">
          <img :src="item.icon_image">
          <p class="service_name">{{item.title}}</p>
          <!-- <a :href="item.link" class="service_link">{{item.link}}</a> -->
        </nuxt-link>
      </li>
    </ul>
  </section>
</template>

<script>
import workList from '../components/worklist.js'

export default {
  data () {
    return {
      list: workList
    }
  }
}
</script>


<style scoped>
  section {
    padding: 56px 0;
    background-image: url('../static/contentBg02.png');
  }
  ul {
    display: flex;
    margin: 0 auto;
    width: 50%;
  }
  li {
    list-style: none;
  }
  img {
    margin-bottom: 7px;
    width: 60%;
  }
  .disc {
    font-size: 12px;
  }
  .service_name {
    font-size: 16px;
    font-weight: 600;
    margin-bottom: 35px;
  }
  .service_link {
    color: #666;
    font-size: 10px;
    text-decoration: none;
    margin-bottom: 14px;
  }
  .title {
    font-size: 48px;
    color: #403A6D;
    margin: 35px 0;
  }
  .link {
    text-decoration: none;
    color: black;
  }
</style>
