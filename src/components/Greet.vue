<template>
    <h2> Hello {{ username }} my wishes are: {{ wish }} </h2>
</template>

<script>
export default {
    name: 'GreetHello',
    props: ['username', 'wish'],
}


</script>

<style>

</style>