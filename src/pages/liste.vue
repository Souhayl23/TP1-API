<template>
    <div class="p-2">
      <h2>Page Liste</h2>
      <Card v-for="unObjet of desObjets" v-bind="unObjet" :key="unObjet.nom"/>
      <!-- <Card v-bind="desObjets[1]"/> -->
    </div>
   
</template>

<script setup lang="ts">
 import Card from '../components/card.vue';
 import Maisons from '../assets/maisons.json';
 const props = defineProps({
  foo: String
});



const desObjets = [{nom:"Villa France",
    prix: 45,
    favori: false,
    image: "./une.jpg", // les images sont simplement l'URL absolue (depuis la racine, débute par '/' )
    nbrSDB: 2,},
    
  {nom:"Villa Italie",
    prix: 55,
    favori: false,
    image: "./une2.jpg", // les images sont simplement l'URL absolue (depuis la racine, débute par '/' )
    nbrSDB: 3,},
    {

    }
];

</script>


