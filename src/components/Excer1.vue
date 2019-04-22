<template>
  <div id="Excer1">
    <h1>Excercise 1 : </h1>
    <b-button variant="warning" @click="Switch">Switch</b-button>
    <p v-if="onsWitch">Show/Hide</p>
    <p v-show="onsWitch">Show/Hide</p>

  </div>
</template>

<script>
export default {
  data() {
    return {
      onsWitch: false
    };
  },
  methods: {
    Switch() {
      this.onsWitch = !this.onsWitch;
    }
  }
};
</script>

<style>
#Excer1 {
  font-family:  Arial;
  text-align: center;
  color:blueviolet;
  margin-top: 60px;
}
div h1{
  color: aqua;
}
div p {
  margin-left: 20%;
}
</style>
