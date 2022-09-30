<script setup lang="ts">
import Card from "../components/card.vue";
import { supabase } from "../supabase";
console.log("supabase :", supabase); // pour vérifier et "garder" supabase dans le code
let { data: maisons, error } = await supabase.from('Maison').select('*')
console.log(maisons);
</script>

<template>
    <div class="p-2">
      <h2>Page List-supabase</h2>
      <div>     
         <Card
       v-for="maison in maisons"
       :key="maison.nom"
       v-bind="maison"/>
       </div>
      
    </div>
   
</template>


