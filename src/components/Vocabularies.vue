<template>
    <div>

        <div class="paginate">

            <nav aria-label="Page navigation">
                <ul class="pagination justify-content-center">
                    <li class="page-item disabled">
                        <a class="page-link" href="#" tabindex="-1">Previous</a>
                    </li>
                    <li class="page-item"><a class="page-link" href="#">1</a></li>
                    <li class="page-item active"><a class="page-link" href="#">2</a></li>
                    <li class="page-item"><a class="page-link" href="#">3</a></li>
                    <li class="page-item">
                        <a class="page-link" href="#">Next</a>
                    </li>
                </ul>
            </nav>

        </div>

        <div>

            <ul class="list-group" v-bind:key="vocabulary.id" v-for="vocabulary in vocabularies">
                <li class="list-group-item">
                    <router-link :to="{ name: 'vocabulary', params: { vocabularyId: vocabulary.id }}">
                        {{ vocabulary.title }}
                    </router-link>
                </li>
                
                <!-- <Vocabulary v-bind:vocabulary="vocabulary"/> -->
            </ul>
        </div>
        
        
    </div>

</template>

<script>

import Vocabulary from './Vocabulary.vue' 

export default {

    name: 'Vocabularies',

    components: {
        Vocabulary
    },

    props: ["vocabularies"]
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

    .paginate{
        margin: 20px;
    }

</style>
