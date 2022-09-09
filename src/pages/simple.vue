<template>
    <div class="p-2">
      <h2>Page Simple</h2>
      <Card image="/une.jpg" />
    </div>
   
</template>

<script setup lang="ts">
 import Card from '../components/card.vue';
 const props = defineProps({
  foo: String
})

</script>

