<script setup lang="ts">
// import { onMounted, ref } from 'vue'
import { RouterView } from 'vue-router'
import AppHeader from '@/components/AppHeader.vue'

// const mobileMenuOpen = ref(false)
/* To enable once supabase setup is ready
import { supabase } from './supabase'
const session = ref()
onMounted(() => {
  supabase.auth.getSession().then(({ data }) => {
    session.value = data.session
  })
  supabase.auth.onAuthStateChange((_, _session) => {
    session.value = _session
  })
})
*/
</script>

<template>
  <AppHeader />
  <main class="px-7 py-14">
    <RouterView />
    <footer class="flex items-center">
      Proudly maintained by Ignotus 2022-ongoing
    </footer>
  </main>

</template>