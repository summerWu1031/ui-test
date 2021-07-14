<template>
<Button>123</Button>
<Tabs v-model:selected="x">
  <Tab title="导航1">内容1</Tab>
    <Tab title="导航2">内容2</Tab>
</Tabs>
</template>

<script>
import {Button,Tabs,Tab} from 'ss-ui-1031'
import 'ss-ui-1031/dist/lib/ss.css'
import {ref} from'vue'
export default {
  name: 'App',
  components: {
    Button,
    Tabs,
    Tab
  },
   setup() {
    const x = ref('导航2')
    return {
      x
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
