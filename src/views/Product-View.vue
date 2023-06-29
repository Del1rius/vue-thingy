<template>
    <div v-if="product" class="product_details">
        <img :src="product.img" :alt="product.name">
        <div>
            <h2>{{ product.name }}</h2>
            <p>Description: {{ product.desc }}</p>
            <p>Price: € {{ product.price }}</p>
        </div>
    </div>
</template>
<script>
export default {
    props: ["id"],

    computed: {
        product() {
            return this.$store.state.product
        }
    },

    mounted() {
        this.$store.dispatch("getProduct", this.id)
    }
}
</script>
<style >
    
</style>