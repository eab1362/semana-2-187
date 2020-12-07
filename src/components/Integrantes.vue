<template>
  <div class="container-fluid">
    <div class="row">
      <div id="integrantes" class="col-sm-6" style="background-color: lavender height: 800px" >
        
        <div v-for="(inte, index) of object"
        :key="index" class="miembros" style="width: 400px height:600px display: grid; grid-template-columns: auto auto auto auto auto; background-color: azure;" >
          <img class="miembro__item" {{ inte.image }} alt="Imagen del Integrante" style="margin: 6px; text-align: justify;  width: 200px; height: 300px;" />
            <h2 style="text-align: center;">{{inte.nombre}}</h2>
            <p class="card-text">{{inte.description}}</p>
            <p class="card-text">{{inte.rol}}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

new Vue ({
  el: '#integrantes',
  data:{
    object: [
      {
        codigo: 1,
        nombre: 'Edgar Andrade',
        descripcion: '',
        rol: 'Desarrollador Backend',
        image: 'https://placeimg.com/200/300/people'
      },

      {
        codigo: 2,
        nombre: 'Fredy Cardona',
        descripcion: '',
        rol: 'Desarrollador Backend',
        image: 'https://placeimg.com/200/300/people'
      },

      {
        codigo: 3,
        nombre: 'Deciret Díaz',
        descripcion: '',
        rol: 'Desarrollador Frontend',
        image: 'https://placeimg.com/200/300/people'
      },
            {
        codigo: 4,
        nombre: 'Hector Gomez',
        descripcion: '',
        rol: 'Desarrollador Frontend',
        image: 'https://placeimg.com/200/300/people'
      },
      {
        codigo: 5,
        nombre: 'Héctor Melgarejo',
        descripcion: '',
        rol: 'Desarrollador Frontend',
        image: 'https://placeimg.com/200/300/people'
      }
    ]
  }
});
</script>

<style scoped>

</style>
