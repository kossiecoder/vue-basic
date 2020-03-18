<template>
  <div>
    <h1>This is Home page</h1>
    <!-- <form action=""> -->
      <InputField v-model="name" />
      <br><button @click="updateName">Submit</button>
    <!-- </form> -->
    {{ name }}
  </div>
</template>

<script>
import InputField from '@/components/InputField.vue';
export default {
  components: {
    InputField
  },
  data() {
    return {
      name: 'Kossie Coder'
    }
  },

  beforeCreate() {
    console.log('beforeCreate', this.name);
  },

  created() {
    console.log('created', this.name);
  },
  beforeMount() {
    alert('beforeMount')
  },
  mounted() {
    alert('mounted')
  },
  beforeUpdate() {
    alert('beforeUpdate')
  },
  updated() {
    alert('updated')
  },
  beforeDestroy() {
    alert('beforeDestroy')
  },
  destroyed() {
    alert('destroyed')
  },
  methods: {
    updateName() {
      this.name = 'hello';
    }
  }
}
</script>

<style scoped>
h1 {
  color: red;
}
</style>