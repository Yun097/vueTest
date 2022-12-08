<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld title="速度" msg="~">
    <HelloWorld title="可以" msg="QQ">
    <HelloWorld title="慢一點嗎" msg="Q_Q">
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
