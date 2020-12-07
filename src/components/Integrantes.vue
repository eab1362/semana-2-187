<template>
        <div class="container">
             <div class="row">
            <div class="integrantes-container" v-for="(Itemtem, index) in items" :key="index" >
<div class="col-sm">
                <teamCard
                    v-bind:image="Itemtem.image"
                    v-bind:nombre="Itemtem.nombre"
                    v-bind:descripcion="Itemtem.descripcion"
                    v-bind:rol="Itemtem.rol"
                />
</div>
            </div>
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

    data(){
        return{
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
    };
    },
};
</script>