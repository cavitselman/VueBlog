<template>
    <div>
        <app-header></app-header>
        <router-view></router-view>
    </div>
</template>

<script>
    import AddBlog from './components/add-blog.vue'
    import ShowBlogs from './components/show-blogs.vue'
    import ListBlogs from './components/list-blogs.vue'
    import Header2 from './components/header2.vue'

    export default {
        components: {
            "add-blog": AddBlog,
            "show-blogs": ShowBlogs,
            'list-blogs': ListBlogs,
            'app-header': Header2,
        },
        data() {
            return {

            }
        }
    }
</script>

<style scoped>
</style>