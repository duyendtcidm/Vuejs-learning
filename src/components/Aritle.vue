<template>
    <div>
        <h2> Aritcle Component </h2>
        <h2> {{ title }} </h2>
        <h3> Like {{ likes }} </h3>
        <h4> Publish status: {{isPublish ? 'Yes' : 'No'}} </h4>
        <h2> BlogPost {{ blogpost }} </h2>
    </div>
</template>

<script>
    export default {
        name: 'ArticleEssay',
        props: {
            title: {
                type: String,
                required: true,
                default: 'Harry Potter',
            },
            likes: Number,
            isPublish: Boolean,
            blogpost: [],

        },
    }
</script>

<style lang="scss" scoped>

</style>