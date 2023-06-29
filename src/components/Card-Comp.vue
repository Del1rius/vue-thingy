<template>
<div class="container">
    <!-- <h2 class="text-white text-center display-3">Products: </h2> -->
    <div class="card mx-auto my-2">
            <router-link :to="{name: 'product', params:{id: product.id}}">
            <div class="card bg-black text-white border-white border-2 text-center ">
            <img :src="product.img" :alt="product.name">
            <h2 class="fs-4">
                {{ product.name }}
            </h2>
            <div class="card-body m-2">
            <p>Description: {{ product.desc }}</p>
            <p>Price: € {{ product.price }}</p>
            </div>
            </div>
            </router-link>
    </div>
</div>
</template>
<script>
export default {
    props: ["product"]
}
</script>
<style scoped>
img {
    height: 400px !important;
}
.card {
    width: 400px;
}
a {
    text-decoration: none;
}

</style>