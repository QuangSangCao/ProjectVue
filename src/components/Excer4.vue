<template>
  <div id="Excer4">
      <input type="number" v-model="Input">
      <b-button variant="warning" @click="tang()">Tang</b-button>
      <b-button variant="warning" @click="giam()">Giam</b-button>
      <p>Total:{{total}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      total: null
      
    };
  },
  methods: {
    tang() {
      this.total = this.total + parseInt(this.Input);
    },
    giam() {
      this.total = this.total - parseInt(this.Input);
    }
  }
};
</script>

<style>

</style>
