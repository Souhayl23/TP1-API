<template>
    <div class="p-2">
      <h2>Page Simple</h2>
      <Card v-bind="unObjet0"/>
      <Card v-bind="unObjet1"/>
    </div>
   
</template>

<script setup lang="ts">
 import Card from '../components/card.vue';
 const props = defineProps({
  foo: String
});



const unObjet0 = {nom:"Villa France",
    prix: 45,
    favori: false,
    image: "./une.jpg", // les images sont simplement l'URL absolue (depuis la racine, débute par '/' )
    nbrSDB: 2,}
const unObjet1 = {nom:"Villa Italie",
    prix: 55,
    favori: false,
    image: "./une2.jpg", // les images sont simplement l'URL absolue (depuis la racine, débute par '/' )
    nbrSDB: 3,}

</script>


