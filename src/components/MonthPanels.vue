<template>
  <div class="expansion-panels">
    <ExpansionPanel
      v-for="month in months"
      :key="month.name"
      :title="month.name"
      :text="month.description"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import ExpansionPanel from './ExpansionPanel.vue'

const months = ref([
  { name: 'January', description: 'Named after Janus, the Roman god of doors and gates.' },
  { name: 'February', description: 'Named after Februa, an early Roman festival and cleansing ritual.' },
  { name: 'March', description: 'Named after Mars, the Roman god of war.' },
  { name: 'April', description: 'Possibly derived from the Latin word "aperire," meaning "to open," referring to the opening of buds in spring.' },
  { name: 'May', description: 'Named after Maia, an earth goddess of growing plants.' },
  { name: 'June', description: 'Named after Juno, the Roman goddess of marriage and childbirth.' },
  { name: 'July', description: 'Named after Julius Caesar.' },
  { name: 'August', description: 'Named after Augustus Caesar.' },
  { name: 'September', description: 'From the Latin "septem," meaning seven.' },
  { name: 'October', description: 'From the Latin "octo," meaning eight.' },
  { name: 'November', description: 'From the Latin "novem," meaning nine.' },
  { name: 'December', description: 'From the Latin "decem," meaning ten.' }
])
</script>

<style scoped>
.expansion-panels {
  max-width: 600px;
  margin: 40px auto;
}
</style>
