<template>
  <div id="Excer2">
    <h1>Excercise 2 : </h1>
      <b-button variant="warning" @click="addItems">Add</b-button>
    <ul>
      <li v-for="(item, index) in items" :key="index" :class="setColor(index)">{{index}}</li>
    </ul>
    
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: []
    };
  },
  methods: {
    addItems() {
      this.items.push("add");
    },
    setColor(index) {
      if (index % 2 == 0) {
          return "sochan";
      } else {
          return "sole";
      }
    }
  }
};
</script>

<style scope>
.sole {
    background-color: red;
    border-radius: 30px;
    text-align: center;
    font-family:  Arial;
    display: block;
}
.sochan{
    background-color: blue;
    border-radius: 30px;
    text-align: center;
    font-family:  Arial;
    display: block;
}
#Excer2 {
  font-family:  Arial;
  text-align: center;
  color:rgb(230, 199, 24);
  margin-top: 60px;
}
div h1{
  color: aqua;
}
</style>
