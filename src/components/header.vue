<template>
    <header>
        <h1 v-on:click="changeTitle">{{ titlex }}</h1>
    </header>
</template>

<script>
    export default {
        props: {
            titlex: {
                type: String,
                required: true
            }
        },
        data() {
            return {
                titlex:"Header Başlık"
            }
        },
        methods: {
            changeTitle: function () {
                this.$emit("basligiDegistir", "Alt Bileşen Tarafından Değiştirilen Başlık")
            }
        }
    }
</script>

<style scoped>
    header {
        background: lightgreen;
        padding: 10px;
    }

    h1 {
        color: #222;
        text-align: center;
    }
</style>