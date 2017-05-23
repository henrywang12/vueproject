<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2> a  => {{ a }}</h2>
    <ul>
      <li v-for="item in items" v-bind:class="{finished:item.isFinished}">
        {{item.label}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data: function () {
    return {
      title: 'this is a todo list',
      items: [
        {label: 'coding', isFinished: false},
        {label: 'walking', isFinished: true}
      ],
      msg: 'Welcome to Your Vue.js App'
    }
  },
  computed: {
    a: function () {
      return this.a + 1
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
