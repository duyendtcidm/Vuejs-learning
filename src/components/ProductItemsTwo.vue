<template>
    <div>
        <h2>Product list 2</h2>
        <ul>
            <li v-for="product in products" :key="product.name">{{product.index}} {{product.name}}  {{ product.price }}</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name:'ProductListTwo',
        props: ['products'],
    }
</script>

<style lang="scss" scoped>

</style>