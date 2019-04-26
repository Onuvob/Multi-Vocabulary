<template>
  <div id="app">
    <Header/>
    <div class="container">
      <Vocabularies v-bind:vocabularies="vocabularies"/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Vocabularies from './components/Vocabularies.vue'

export default {
  name: 'app',
  components: {
    Header,
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

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
 
}
</style>
