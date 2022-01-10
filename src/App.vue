<template>
  <div class="app">
    <p>{{ name }} - {{ age }}</p>
    <button @click="changeName('zel')">change name</button>
    <button @click="changeAge(47)">change age</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {},
  data() {
    return {
      name: "Link",
      age: 50 as number | string
    }
  },
  methods: {
    changeName(name: string) {
      this.name = name;
    },
    changeAge(age: number | string) {
      this.age = age;
    }
  }
});
</script>

<style>

</style>
