<template>
    <div class="p-2">
      <h2>Page Simple</h2>
      <Card v-for="unObjet of desObjets" v-bind="unObjet" :key="unObjet.nom"/>
      <!-- <Card v-bind="desObjets[1]"/> -->
    </div>
   
</template>

<script setup lang="ts">
 import Card from '../components/card.vue';
 const props = defineProps({
  foo: String
});



const desObjets = [{nom:"une card de maison",
    prix: 45,
    favori: false,
    image: "./une.jpg", // les images sont simplement l'URL absolue (depuis la racine, débute par '/' )
    nbrSDB: "Number",},
    
  {nom:"card",
    prix: "Number",
    favori: "Boolean",
    image: "./une.jpg", // les images sont simplement l'URL absolue (depuis la racine, débute par '/' )
    nbrSDB: "Number",},
    {

    }
];

</script>


