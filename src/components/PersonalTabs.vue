<template>
  <q-tabs v-model="tab" class="text-primary" align="justify">
    <q-tab name="skills" label="Skills" />
    <q-tab name="education" label="Eduication" />
    <q-tab name="experience" label="Experience" />
    <q-tab name="interests" label="Interests" />
  </q-tabs>
  <q-separator />
  <div class="q-mt-md">
    <q-tab-panels v-model="tab" animated>
      <q-tab-panel name="skills">
        <Skills />
      </q-tab-panel>
      <q-tab-panel name="education">
        <Education />
      </q-tab-panel>
      <q-tab-panel name="experience">
        <Experience />
      </q-tab-panel>
      <q-tab-panel name="interests">
        <Interests />
      </q-tab-panel>
    </q-tab-panels>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import Skills from '../pages/Skills.vue'
import Education from '../pages/Education.vue'
import Experience from '../pages/Experience.vue'
import Interests from '../pages/Interests.vue'

const tab = ref('skills')
</script>
