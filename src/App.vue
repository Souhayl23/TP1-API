<template>
  <nav>
    <h4 class="text-xl">
      <Bars3Icon class="inline-block h-5 w-5 text-blue-500" />
      menu (dans <code class="font-mono">/src/App.vue</code>)
    </h4>
    <ul>
      <li>
        <router-link class="text-red-600 underline" to="/simple">
          lien vers
          <code class="font-mono">simple.vue</code>
        </router-link>
        
      </li>
      <li>        <router-link class="text-blue-600 underline" to="/liste">
          lien vers
          <code class="font-mono">liste.vue</code>
        </router-link></li>
        <li>        <router-link class="text-green-600 underline" to="/liste-fetch">
          lien vers
          <code class="font-mono">liste-fetch.vue</code>
        </router-link></li>
        <li>
        <router-link class="text-yellow-600 underline" to="/edit/new">
          lien vers
          <code class="font-mono">new.vue</code>
        </router-link></li>

        <li>
        <router-link class="text-orange-700 underline" to="connexion">
         lien pour se connecter 
        </router-link>
      </li>
        
    </ul>
  </nav>

  <!-- Affiche les pages -->
  <Suspense>
  <router-view class="m-2 border-2 p-2" />
</Suspense>

</template>

<script setup lang="ts">
import { Bars3Icon } from '@heroicons/vue/20/solid'
</script>
