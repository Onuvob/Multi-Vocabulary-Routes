<template>
    <div class="jumbotron">
        <h1 class="display-4">{{ word }}</h1>
        <p class="lead">{{ example }}</p>
        <hr class="my-4">
        <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>
        <p class="lead">
            <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
        </p>
    </div>
</template>

<script>


export default {
    data() {
        return {
            word: "",
            example:""
        }
    },
    mounted () {
        this.init()
    },

    methods: {
        init () {
            this.word = this.$route.params.vocabulary.word
            this.example = this.$route.params.vocabulary.example
        },
    }
}
</script>

<style>

</style>
