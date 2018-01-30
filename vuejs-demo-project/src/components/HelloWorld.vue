<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h1>{{ msg1 }}</h1>
    <h1>{{ msg2 }}</h1>
    <ol>
      <li v-for="todo in todos">
        {{ todo.text }}
      </li>
    </ol>
    <span v-if="seen">Now you see me</span>
    <p>{{ message }}</p>
    <button @click="checkFunc">Reverse Message</button>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data () {
      return {
        msg: 'Welcome to Your Vue.js App',
        msg1: 'Welcome to Your Vue.js App',
        msg2: 'Welcome to Your Vue.js App',
        todos: [
          {text: 'Learn JavaScript'},
          {text: 'Learn Vue'},
          {text: 'Build something awesome'}
        ],
        seen: true,
        message: 'Hello Vue.js!'
      }
    },
    methods: {
      checkFunc(){
        console.log('All is working!');
      },
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
