<template>
  <div id="app">
    <Header />
    <Skills v-bind:skills="skills"/>
  </div>
</template>

<script>
import Header from './components/layout/Header.vue'
import Skills from './components/Skills.vue'
import StarRating from 'vue-star-rating'

export default {
  name: 'app',
  components: {
    Header,
    Skills,
    StarRating
  },
  data() { 
    return {
      skills: [
        {
          id: 1,
          title: "java",
          progress: 4/5
        },
        {
          id: 2,
          title: "C/C++",
          progress: 3/5
        },
        {
          id: 3,
          title: "Web development",
          progress: 3/5
        },
        {
          id: 4,
          title: "VHDL",
          progress: 2/5
        },
        {
          id: 5,
          title: "SQL",
          progress: 3/5
        }
      ]
    }
  }
}
</script>

<style>
  * {
    box-sizing: border-box;
    padding: 0px;
    margin: 0px
  }
  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
  }
</style>
