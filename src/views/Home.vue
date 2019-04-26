<template>
  <div class="home">
    <div class="container">
      <Vocabularies v-bind:vocabularies="vocabularies"/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Vocabularies from '../components/Vocabularies.vue' 

export default {
  name: "home",
  components: {
    Vocabularies
  },

  data() {
    return{
      vocabularies:[
        {
          id:	1,
          title:	"delectus aut autem",
          completed:	false
        },
        {
          id:	2,
          title:	"quis ut nam facilis et officia qui",
          completed:	false
        },      
        {
          id:	3,
          title:	"fugiat veniam minus",
          completed:	false
        }        

      ]
    }
  }
};
</script>
