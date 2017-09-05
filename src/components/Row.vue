<template>
  <tr>
    <td v-for="(key, index) in dados" :key="key">{{key}}</td>
  </tr>
</template>
<script>
  export default{
    name: 'MyRow',
    props: ['dados']
  }
</script>
