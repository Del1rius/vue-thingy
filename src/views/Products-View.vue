<template>
    <div v-if="products" class="flex-container">
        <CardComp v-for="product of products" :key="product.id" :product="product"/>
    </div>
    <div v-else>Loading...</div>
</template>
<script>
import CardComp from '@/components/Card-Comp.vue';
export default {
    computed: {
        products() {
            return this.$store.state.products
        }
    },

    mounted() {
        this.$store.dispatch("getProducts")
    },

    components: {CardComp},
}
</script>
<style>
.flex-container{
    background-color: #BD2C2C;
    margin: 0;
    padding: 0;
    width: 100%;
}
   
</style>