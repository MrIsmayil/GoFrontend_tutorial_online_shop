<template>
    <div id="Home">
        <main-wrapper/>
       

    </div>
</template>

<script>
import mainWrapper from "@/components/main-wrapper"
export default {
    name: "Home",
    components: {
        mainWrapper
    },
    props: {},
    data() {
        return {
            title: "Home!",

        }
    },

    computed: {},
    methods: {},
    watch: {},
    mounted() {
        console.log("Hello it is Home!");
    },
    
}
</script>

<style scoped>

</style>