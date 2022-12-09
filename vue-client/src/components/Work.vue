<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
    </div>

    <!-- Loop thru projects and display -->
    <span v-for="n in 10">
        <Project :msg="'Project ' + n" />
    </span>


</template>
  
<script>
import Project from '@/components/Project'

export default {
    name: 'Work',
    components: {
        Project
    },
    props: {
        msg: String
    }
}
</script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
    margin: 40px 0 0;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42b983;
}
</style>