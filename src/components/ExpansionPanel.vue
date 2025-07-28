<template>
  <div class="panel">
    <div class="panel-header" @click="expanded = !expanded">
      <h2>{{ title }}</h2>
      <span>{{ expanded ? '-' : '+' }}</span>
    </div>
    <div v-if="expanded" class="panel-body">
      <p>{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ExpansionPanel',
  props: {
    title: String,
    text: String
  },
  data() {
    return {
      expanded: false
    }
  }
}
</script>

<style scoped>
.panel {
  border: 1px solid #ccc;
  border-radius: 8px;
  margin-bottom: 16px;
  background: #f9f9f9;
  box-shadow: 0 2px 4px rgba(0,0,0,0.04);
}
.panel-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer;
  padding: 16px;
  background: #e3e3e3;
  border-radius: 8px 8px 0 0;
}
.panel-body {
  padding: 16px;
}
</style>
