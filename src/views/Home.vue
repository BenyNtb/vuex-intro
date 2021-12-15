<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <Component1 msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Component1 from '@/components/Component1.vue'

export default {
  name: 'Home',
  components: {
    Component1,
  }
}
</script>
