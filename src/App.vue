<template>
  <div id="app">
    <Header />
    <div class="SkillSet">
      <header class="Skillset">Skillset:</header>
      <Skills v-bind:skills="skills"/>
    </div>
  </div>
</template>

<script>
import Header from './components/layout/Header.vue'
import Skills from './components/Skills.vue'

export default {
  name: 'app',
  components: {
    Header,
    Skills
  },
  data() { 
    return {
      skills: [
        {
          id: 1,
          title: "Java",
          progress: 4
        },
        {
          id: 2,
          title: "C/C++",
          progress: 3
        },
        {
          id: 3,
          title: "Web development",
          progress: 3
        },
        {
          id: 4,
          title: "VHDL",
          progress: 2
        },
        {
          id: 5,
          title: "SQL",
          progress: 3
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
  .SkillSet {
    position: absolute;
    right: 10px;
  }
</style>
