<template>
    <div>
        <div v-bind:key="skill.id" v-for="skill in skills">
            <Skill v-bind:skill="skill"/>
        </div>
    </div>
</template>

<script>
import Skill from './Skill.vue';

export default {
    name:'Skills',
    components: {
        Skill
    },
    props: ["skills"]
}
</script>

<style scoped>
    *  {
        border: 1px solid black;
    }
</style>
