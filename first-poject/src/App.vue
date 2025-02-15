<template>
  <h3>{{ title }}</h3>
  <p>{{ anons }}</p>
  <button type="button" @click="userData()">Send</button>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      title: 'Title!',
      anons: 'This is anons'
    };
  },
  methods: {
    userData(word='New word') {
      this.title = 'New title';
      this.anons = word;
    }
  }
};
</script>

<style scoped>
h3 {
  font-weight: lighter;
}

p {
  color: red
}
</style>
