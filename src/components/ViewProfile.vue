<template>
    <div class="view-profile">
        <h1>Profile {{id}}</h1>
        
    </div>
</template>

<script>
export default {
    name: 'ViewProfile',
    data() {
        return {
           id: this.$route.params.id,
        }
    },
    methods: {
        updateThings() {
            this.id = this.$route.params.id
       }
},
    watch: {
        $route: 'updateThings'
    }
}
</script>


<style>

</style>
