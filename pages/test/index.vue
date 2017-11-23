<template>
  <div>
    <Logo/>
    <button @click="addItem">add</button>
    <ul>
      <ListItem
        v-for="(item, index) in list"
        :key="item.name"
        @click="onClick(item.name, $event)"
        v-bind:name="item.name"
        >
      </ListItem>
      </li>
    </ul>
    <input v-model="text">
      {{text}}
  </div>
</template>

<script>
import Logo from '../../components/Logo.vue'
import ListItem from '../../components/ListItem.vue'

export default {
  data () {
    return {
      list: [
        {
          name: 'chip'
        },
        {
          name: 'dale'
        },
        {
          name: 'gadget'
        }
      ],
      text: 'yuridayo'
    }
  },
  methods: {
    onClick (name, e) {
      console.log(name, e)
    },
    addItem () {
      this.list.push({
        name: 'pyoro'
      })
    }
  },
  components: {
    Logo,
    ListItem
  }
}
</script>
