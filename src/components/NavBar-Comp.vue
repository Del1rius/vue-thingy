<template >
    <div>
      <router-link to="/">Home</router-link>  
      <router-link to="/about">About</router-link>
      <router-link to="/products">Products</router-link>
      <router-link to="/contact">Contact</router-link>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
 div{
    background-color: black;
    padding: 30px;
 }

 a {
    text-decoration: none;
    color: crimson;
    text-align: center;
    font-size: 25px;
    padding: 20px;
    margin: 20px;
 }   

 a:hover {
    background-color: crimson;
    color: lavenderblush;
    border-radius: 20px;
 }
</style>