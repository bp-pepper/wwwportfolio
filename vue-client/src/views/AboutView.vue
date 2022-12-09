<template>
  <div class="about">
    <About msg="About" />
    <h1>This is an about page</h1>
  </div>
</template>

<script>
import About from '@/components/About.vue'

export default {
  name: 'AboutView',
  components: {
    About
  }
}

</script>
