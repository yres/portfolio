<template>
  <section>
    <ul>
      <li v-for="(item, key) in list" :key="key">
        <a :href="item.link">
          <img :src="item.image">
        </a>
      </li>
    </ul>
  </section>
</template>

<<script>
import socialList from '../components/socialList.js'

export default {
  data () {
    return {
      list: socialList
    }
  }
}
</script>

<style scoped>
section {
  padding: 28px 0;
  background: #403A6D;
}
ul {
  display: flex;
  width: 20%;
  margin: 0 auto;
}
li {
  list-style: none;
  margin: 0 auto;
}
</style>


</style>

