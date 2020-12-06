<template>
  <div  class="container-fluid" >
    
    {{noticia.author}}  

  </div>
</template>

<script>

export default {
  name: 'Items',
  props:{
  'noticia':Object
  },
  data (){
   return{}
  },
  created (){
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>