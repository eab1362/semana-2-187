<template>
  <footer class="p-2 bg-info"> 
        <div class="row">
      <div class="col-sm-6">
        <p class="text-justify">
          Este sitio web fue desarrollado para el proyecto
          <b>Misión TIC 2022</b>, en articulación con la
          <b>Universidad Tecnológica de Pereira</b>.
        </p>
        <p class="text-justify">
          Repositorio GitHub:
          <a href="https://github.com/03DEIMOS/semana-1-187"
            >Ir al Repositorio del grupo 187</a
          >
        </p>
      </div>
      <div class="col-sm-6 ">
       <h6 class="text-sm-left">Contáctenos:</h6>
        <div class="row">
      <small class=" col-sm-4 text-sm-left p-2">Edgar Andrade: <a href="#">305 723 2467</a></small>
      <small class=" col-sm-4 text-sm-left p-2">Fredy Cardona: <a href="#">311 295 2533</a></small>
      <small class=" col-sm-4 text-sm-left p-2">Deciret Díaz: <a href="#">301 274 3500</a></small>
      <small class=" col-sm-4 text-sm-left p-2">Héctor Gómez: <a href="#">318 404 3862</a></small>
      <small class=" col-sm-4 text-sm-left p-2">Héctor Melgarejo: <a href="#">302 279 3723</a></small>

        </div>
      </div>
    </div>
  </div>
    
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
