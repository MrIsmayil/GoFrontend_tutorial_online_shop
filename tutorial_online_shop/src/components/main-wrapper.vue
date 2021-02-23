<template>
    <div class="main-wrapper">      
         <catalog/>
    </div>
</template>

<script>
import Catalog from "./catalog";
// import Cart from "./cart"

export default {
    name: "main-wrapper",
    components: {
        Catalog,
        
        
    },
    props: {},
    data() {
        return {
            title: "Main wrapper!",

        }
    },

    computed: {},
    methods: {},
    watch: {},
    mounted() {
        console.log("Hello I am aktive!");
    },
}
</script>

<style>
.main-wrapper {
    max-width: 900px;
    margin: 0 auto;
    justify-content: flex-start;
}


</style>