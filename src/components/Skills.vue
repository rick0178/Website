<template>
    <div>
        <header class="Skillset">Skillset:</header>
        <div v-bind:key="skill.id" v-for="skill in skills">
            <h3>{{skill.title}}</h3>
        </div>
    </div>
</template>

<script>
export default {
    name:'Skills',
    props: ["skills"]
}
</script>

<style scoped>
 
</style>
