<template>
    <div class="jumbotron">
        <h1 class="display-4">{{ title }}</h1>
        <p class="lead">This is a simple hero unit, a simple jumbotron-style component for calling extra attention to featured content or information.</p>
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
            id: "",
            title:""
        }
    },
    mounted () {
        this.init()
    },

    methods: {
        init () {
            this.id = this.$route.params.vocabulary.id
            this.title = this.$route.params.vocabulary.title
        },
    }
}
</script>

<style>

</style>
