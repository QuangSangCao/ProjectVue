<template>
  <div id="Excer3">
    <h1>Excercise 3 : </h1>
    <ul>
     
      <li v-for="(item, index) in items" :key="index">
        <div
          v-for="(value, key, index) in item"
          :key="index"
        >{{key}}:{{value}}({{index}}) {{setNumber(value)}}</div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [{ a: 1, b: 2 }, { a: 2, b: 4 }]
    };
  },
  methods: {
    setNumber(value) {
      if (value % 2 == 0) {
        return "so chan";
      } else {
        return "so le";
      }
    }
  }
};
</script>

<style>
div ul li {
  text-align: center;
  color: darkgoldenrod;
}
div h1{
  color: aqua;
  text-align: center;
}
</style>
