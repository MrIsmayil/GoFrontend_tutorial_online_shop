<template>
    <div class="Catalog-item">
         <h1> {{ title }} </h1>
         <p>Price: 100</p>
         <button>Add to cart</button>

    </div>
</template>

<script>
export default {
    name: "Catalog-item",
    props: {},
    data() {
        return {
            title: "Item 1!",

        }
    },

    computed: {},
    methods: {},
    watch: {},
    mounted() {
        console.log("Hello Catalog Item is aktive!");
    },
}
</script>

<style scoped>

</style>