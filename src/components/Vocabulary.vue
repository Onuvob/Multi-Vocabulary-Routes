<template>
    <div class="jumbotron">
        <h1 class="display-4">{{ word }}</h1>
        <p class="lead" v-if="synonym"><mark>Synonym:</mark> <i>{{ synonym }}</i></p>
        <hr class="my-4">
        <p v-if="example"><mark>Example:</mark> {{ example }}</p>
        
        <youtube class="mt-5" v-if="video" :video-id="video"></youtube>

        
    </div>
</template>

<script>


export default {
    data() {
        return {
            word: "",
            synonym: "",
            example: "",
            video: ""
        }
    },
    mounted () {
        this.init()

        
    },

    methods: {
        init () {
            this.word = this.$route.params.vocabulary.word
            this.synonym = this.$route.params.vocabulary.synonym
            this.example = this.$route.params.vocabulary.example
            this.video = this.$youtube.getIdFromURL(this.$route.params.vocabulary.video)
        },
    }
}
</script>

<style>

</style>
