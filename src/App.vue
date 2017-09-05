<template>
  <my-table :css_class="css" :headers="head">
    <my-row v-for="(key, index) in dados" :key="key" :dados="dados[index]"></my-row>
  </my-table>
</template>
<script>
import './style.css'
import MyTable from './components/Table.vue'
import MyRow from './components/Row.vue'
export default {
  data () {
    return {
      head: ['um', 'dois'],
      dados: [[1, 2], [3, 4]],
      css: ['table']
    }
  },
  name: 'app',
  components: {
    MyTable,
    MyRow
  }
}
</script>
