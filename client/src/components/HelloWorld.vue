<template>
  <div class="hello">
   </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  background-image: linear-gradient(rgba(0,0,0,0.6),rgba(0,0,0,0.5)),url("https://images.pexels.com/photos/1482803/pexels-photo-1482803.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500") ;
  height: 94.5vh;
  background-size: cover;
  width:60%;
  
  background-repeat: no-repeat;
}

a {
  color: #42b983;
}
</style>
