<template>
  <div class="home">
    <img alt="BP logo" src="../assets/my-name-is.jpg">
    <Home msg="Welcome to my Portfolio" />
  </div>
</template>

<script>
// @ is an alias to /src
import Home from '@/components/Home'

export default {
  name: 'HomeView',
  components: {
    Home
  }
}
</script>
