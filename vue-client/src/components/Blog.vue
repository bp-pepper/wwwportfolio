<template>
  <div>
    <h1>Blog</h1>
    <p class="lead">{{ fetch_status }}</p>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  name: 'Blog',
  data() {
    return {
      fetch_status: "fetching"
    }
  },
  created() {
    axios({
      method: 'get',
      url: 'http://localhost:9000',
    })
      .then((response) => {
        this.fetch_status = "success"
        console.log(response.data)
      })
      .catch((error) => {
        this.fetch_status = "failed"
      })
  }
}
</script>


