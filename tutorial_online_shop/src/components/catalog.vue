<template>
    <div class="Catalog">
         <h1> {{ title }} </h1>
         <catalog-item/>

    </div>
</template>

<script>
import CatalogItem from "./catalog-Item"



export default {
    name: "Catalog",
    components: {
        CatalogItem,
    },
    props: {},
    data() {
        return {
            title: "Catalog!",

        }
    },

    computed: {},
    methods: {},
    watch: {},
    mounted() {
        console.log("Hello Catalog is aktive!");
    },
}
</script>

<style scoped>

</style>