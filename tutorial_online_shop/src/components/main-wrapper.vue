<template>
    <div class="Main_wrapper">
         <h1> {{ title }} </h1>

    </div>
</template>

<script>
export default {
    name: "Main-wrapper",
    props: {},
    data() {
        return {
            title: "Hello Vue!",

        }
    },

    computed: {},
    methods: {},
    watch: {},
    mounted() {
        console.log("Hello I am akive!");
    },
}
</script>

<style scoped>

</style>