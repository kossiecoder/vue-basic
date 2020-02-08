<template>
  <div>
    <h1>This is Home page</h1>
    <KossieCoder />
  </div>
</template>

<script>
import KossieCoder from '@/components/KossieCoder.vue';

export default {
  components: {
    KossieCoder
  },

  data() {
    return {
      name: 'Kossie Coder'
    }
  }
}
</script>

<style scoped>
h1 {
  color: red;
}
</style>