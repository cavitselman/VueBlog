<template>
    <footer>
        <p>{{ copyright }} - {{ year }} - {{ titley }}</p>
    </footer>
</template>

<script>
    export default {
        props: {
            titley: {
                type: String,
                required: true
            }
        },
        data() {
            return {
                copyright: "Tüm Hakları Saklıdır. (c)",
                year: 2024
            }
        }
    }
</script>

<style scoped>
    footer {
        background: #222;
        padding: 6px;
    }

    p {
        color: lightgreen;
        text-align: center;
    }
</style>