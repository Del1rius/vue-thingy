<template>
    <div v-if="product" class="product_details">
        <div class="card mx-auto bg-black">
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
        </div>
    </div>
</template>
<script>
export default {
    computed: {
        product() {
            return this.$store.state.product
        },
        id(){
            return this.$route.params.id
        }
    },

    mounted() {
        this.$store.dispatch("getProduct", this.id)
    }
}
</script>
<style scoped>
 .product_details{
    background-color: #BD2C2C;
 }
img {
    height: 400px !important;
}
.card {
    width: 400px;
}
</style>