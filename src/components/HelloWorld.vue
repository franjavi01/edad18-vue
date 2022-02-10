<template>
  <div class="hello">
    <input v-model="ageInput" type="text" />
    <button @click="drive">¿Que edad tienes?</button>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      ageInput: "",
      message: "",
    };
  },
  props: {
    msg: String,
  },
  methods: {
    drive() {
      let age = this.ageInput;
      if (age >= 18) {
        this.message = "Puedes conducir";
      } else {
        this.message = "No puedes conducir";
      }
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
