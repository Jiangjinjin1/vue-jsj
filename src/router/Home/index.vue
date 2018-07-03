<template>
  <main>
    <el-button type="primary" @click.native="hello">primary</el-button>
    <hello></hello>
  </main>
</template>

<script>
  import Vue from 'vue'
  import Component from 'vue-class-component'
  import Hello from '~components/Hello'

  @Component({
    components: {
      Hello
    }
  })
  export default class HomeRoute extends Vue {
    hello () {
      this.$message('Hello Vue')
    }
  }
</script>
