<template>
        <div class="container">
            <div class="integrantes-container" v-for="(Itemtem, index) in Items" :key="index" >

                <teamCard
                    v-bind:image="image"
                    v-bind:nombre="nombre"
                    v-bind:descripcion="descripcion"
                    v-bind:rol="rol"
                />
            </div>
        </div>
</template>

<script>
import teamCard from '@/components/TeamCard'

export default {
    name: 'Integrantes',
    components:{
        teamCard,
    },

    data:{
        items:[
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
        /*return{
            codigo: 1,
            nombre: 'Edgar Andrade',
            descripcion: '',
            rol: 'Desarrollador Backend',
            image: 'https://placeimg.com/200/300/people'
        };*/
    },
};
</script>