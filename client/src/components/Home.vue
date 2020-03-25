<template>

    <div class="container-fluid">
  <div class="row no-gutter">
    <div class="d-none d-md-flex col-md-4 col-lg-6 bg-image">
        <div class="logo"></div>
        <div class="text-container"><div class="text">BBQ Delivery service at the  touch  of a button </div>
        <button class="learnmore" >Learn More</button>
    </div></div>
    <div class="col-md-8 col-lg-6">
      <div class="login d-flex align-items-center py-5">
        <div class="container">
          <div class="row">
            
              <Register/>

              <li v-if="auth==''" class="nav-item">
                    <router-link class="nav-link" to="/login">Login</router-link>
                </li>


              
            
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

</template>
<style scoped>

/* .container{
    width: 40%;
    float: right;
    background-image: linear-gradient(rgba(0,0,0,.5),rgba(0,0,0,.5)),url("https://images.pexels.com/photos/1482803/pexels-photo-1482803.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500");
    height: 95.6vh;
    background-repeat: no-repeat;
    background-size: cover;
} */.bg-image {
  background-image:linear-gradient(rgba(0,0,0,0.8),rgba(0,0,0,0.8)), url('https://images.pexels.com/photos/3646847/pexels-photo-3646847.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260');
  background-size: cover;
  background-position: center;
  height:100vh;
  width:60%;
  margin-top: 0;
  left:0 !important;
  float: left;
}
.logo{
    background-image: url('/images/logo.png');
    z-index: 999;
}
.learnmore{
    padding-bottom: 15px;
    height:35px;
    width:150px;
    border: 5px 5px;
    margin-top:6%;
}
.text{
    /* margin-top:40%;
    margin-left:30%; */
    color: white;
    font-weight:600;
    font-size:45px;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
}
.text-container{
    width:450px;
    height:300px;
    margin-top:38%;
    margin-left:18%;
    
}
</style>
<script>
import Register from './Register'
export default {
    name: 'App',
  components:{
    'Register':Register
  }
}
</script>