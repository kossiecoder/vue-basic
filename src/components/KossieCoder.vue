<template>
    <div>
        <p>{{ name }}</p><br>
        <button @click="updateName">Change Name</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            name: 'Kossie Coder',        
        }
    },

    methods: {
        updateName() {
            this.name = 'Kossie Coder Updated';
        }
    }
}
</script>

<style scoped>

</style>