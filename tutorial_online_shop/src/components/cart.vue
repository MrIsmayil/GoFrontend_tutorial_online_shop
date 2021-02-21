<template>
    <div class="Cart">
         <h1> {{ title }} </h1>

    </div>
</template>

<script>
export default {
    name: "Cart",
    props: {},
    data() {
        return {
            title: "Cart!",

        }
    },

    computed: {},
    methods: {},
    watch: {},
    mounted() {
        console.log("Hello Cart is aktive!");
    },
}
</script>

<style scoped>

</style>