<template>
    <div>
        <h2>Product list 1</h2>
        <ul>
            <li v-for="product in products" :key="product.index">{{product.index}} {{product.name}}  {{ product.price }}</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name:'ProductListOne',
        props: ['products']
    }
</script>

<style lang="scss" scoped>

</style>