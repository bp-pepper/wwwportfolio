<template>
  <div>
    <Blog msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import Blog from '@/components/Blog.vue'

export default {
  name: 'HomeView',
  components: {
    Blog
  }
}
</script>
