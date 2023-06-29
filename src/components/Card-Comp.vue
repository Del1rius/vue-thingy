<template>
<div class="container">
    <h2 class="text-white text-center display-3">Products: </h2>
    <div class="card">
        <router-link :to="{name: 'product', params:{id: product.id}}">
        <img :src="product.img" :alt="product.name">
        <h2>
            {{ product.name }}
        </h2>
        <p>Description: {{ product.desc }}</p>
        <p>Price: € {{ product.price }}</p>
        </router-link>
    </div>
    
</div>
</template>
<script>
export default {
    props: ["product"]
}
</script>
<style>
p {
    text-decoration: none !important;
}
img {
    width: 400px;

}
   .card {
    background-color: black;
    border: 2px black solid;
    height: 400px;

   } 
</style>