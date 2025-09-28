
<script setup>
import PersonalTabs from './components/PersonalTabs.vue'
</script>

<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <div class="q-pa-md flex flex-center">
        <div style="width: 100%; max-width: 1050px;">
          <PersonalTabs />
        </div>
      </div>
    </q-page-container>
  </q-layout>
</template>


<style scoped>
.q-layout {
  min-height: 100vh;
  background: #f5f5f5;
}
</style>