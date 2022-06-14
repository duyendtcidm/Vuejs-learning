<template>
    <div>
        <h2>This is a popup</h2>
        <button @click="$emit('close')">Close popup</button>
    </div>
</template>

<script>
    export default {
        name: 'PopupButton',
        emits: ['close'],
    }
</script>

<style lang="scss" scoped>

</style>