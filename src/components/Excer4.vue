<template>
  <div id="Excer4">
      <h1>Excercise 4 :</h1>
      <input type="number" v-model="Input" >
      <b-button variant="warning" @click="Increase()">Increase</b-button>&nbsp;
      <b-button variant="warning" @click="Decrease()">Decrease</b-button>
      <p>Total:{{total}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      total: 0
      
    };
  },
  methods: {
   Increase() {
      this.total = this.total + parseInt(this.Input);
    },
    Decrease() {
      this.total = this.total - parseInt(this.Input);
    }
  }
};
</script>

<style>
#Excer4{
  width: 80%;
  margin: 0 auto;
  text-align: center;
}
div h1 {
  color: aqua;
}
div p {
  color: violet;
  margin-top: 1%;
  margin-right: 20%;
}
</style>
