<template>
    <div class="p-2">
      <h2>Page List-fetch</h2>
      <div>{{maisons}} </div>
      
    </div>
   
</template>

<script setup lang="ts">
    import Maisons from '../assets/maisons.json';
    const maisons = await fetch('../assets/maisons.json')
    const desObjets = await maisons.json()
  


</script>