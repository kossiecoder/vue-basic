<template>
    <div>
        <p>header</p>
        <slot name="header" :kossie="kossie"></slot>
        <p>Body</p>
        <slot></slot>
        <p>footer
        </p>
    </div>
</template>

<script>
export default {
    props: {
        title: {
            type: String,
            default: 'default title'
        },
        name: {
            type: String,
            default: 'default name'
        },

    },
    data() {
        return {
            kossie: 'coder'
            // name: 'Kossie Coder',        
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