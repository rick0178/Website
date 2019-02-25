<template>
    <div>
        <div class="skill">
            {{skill.title}}
            <star-rating v-model="skill.progress" 
                         v-bind:show-rating="false"
                         v-bind:read-only="true"
                         v-bind:star-size="20">
            </star-rating>
        </div> 
    </div>
</template>

<script>
import StarRating from 'vue-star-rating'

export default {
    name: "Skill",
    components: {
        StarRating
    },
    props: ["skill"]
}
</script>

<style scoped>
    .skill {
        display: flex;
        margin: 5px;
    }
</style>
