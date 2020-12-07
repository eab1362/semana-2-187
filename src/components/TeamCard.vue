<template>
  <div class="integrantes">
    <div class="integrantes-row">
      <img :src="image"/>
      <h1 class ="integrantes-nombre">{{nombre}}</h1>
      <div class="integrantes-descripcion">{{descripcion}}</div>
      <div class="integrantes-rol">{{rol}}</div>
    </div>
  </div>
</template>

<script>

export default{
  name: 'TeamCard',

  props:{
    codigo:{
      type: String,
      require: true,
    },
    nombre:{
      type: String,
      require: true,
    },
    descripcion:{
      type: String,
      require: true,
    },
    rol:{
      type: String,
      require: true,
    },
    image:{
      type: String,
      require: true,
    },
  },
};

/*
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
});*/
</script>

<style scoped>

</style>
