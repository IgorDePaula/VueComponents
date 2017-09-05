<template>
  <div>
    <table :class="classes">
      <th v-for="h in headers">{{h}}</th>
      <slot></slot>
    </table>
  </div>
</template>
<script>
  export default{
    name: 'MyTable',
    props: ['headers', 'css_class'],
    computed: {
      classes () {
        return this.css_class.join(' ')
      }
    }
  }
</script>
