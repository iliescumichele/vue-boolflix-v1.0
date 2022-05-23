<template>
  <div id="app">
    
    <headerComponent />

    <mainComponent />
    
  </div>
</template>

<script>
import axios from 'axios'
import headerComponent from './components/headerComponent.vue'
import mainComponent from './components/headerComponent.vue'

export default {
  name: 'App',
  components: {
    headerComponent,
    mainComponent
  },

  data(){
    return{
      baseURL: 'https://api.themoviedb.org/3/search/movie/',
      apiParams:{
        api_key: '7c7fba51d38f79e494fc734298af352a',
        language: 'it-IT',
        query: 'ciao'
      },
    }
  },

  mounted(){
      axios.get(this.baseURL,{
        params: this.apiParams}
      )
      .then(response => {
        console.log(response.data.results);
      })
      .catch(error =>{
        console.log(error)
      })
  },
}
</script>

<style lang="scss">

  @import './assets/style/general.scss'

</style>
