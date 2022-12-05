<template>
  <div class="container">
    <h1 class="text-center py-3 text-info">
      <span class="badge bg-info">Description of the site </span>
    </h1>
    <div :class="{ 'text-danger': color, 'text-info': !color }">
      <p id="lorem">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dignissimos doloribus
        autem deserunt, praesentium dolor earum? Quasi est ducimus nam voluptas in dolores
        aliquam dolor autem nemo iusto cumque fuga quis dolore enim nostrum laudantium
        recusandae a, nobis, facere atque. Hic ea recusandae assumenda magnam ab dicta
        commodi doloribus?
      </p>
      <button @click="color = !color" type="button" class="btn btn-outline-info px-3">
        Chance text color
      </button>
    </div>

    <hr />
    <button
      id="btn"
      @click="show = !show"
      type="button"
      class="btn btn-outline-info px-3"
    ></button>

    <p v-if="show" class="py-3 text-center">
      &emsp; &#128276; &emsp; &#9989; &emsp; &#9203; &emsp; &#9971; &emsp; &#169; &emsp;
      &#128269; &emsp; &#128190; &emsp; &#9993; &emsp; &#128736; &emsp; &#128465; &emsp;
      &#9940; &emsp; &#10060; &emsp; &#128368; &emsp; &#8986; &emsp; &emsp; &emsp;
    </p>

    <hr />

    <button @click="products" type="button" class="btn btn-outline-success px-3">
      Products
    </button>
    <button @click="write" type="button" class="btn btn-outline-danger px-3">
      Write...
    </button>
    <button @click="finish" type="button" class="btn btn-outline-warning px-3">
      Finish
    </button>
  </div>
</template>

//
<script>
import { write } from "@popperjs/core";

export default {
  data() {
    return {
      show: false,
      color: true,
    };
  },

  methods: {
    // test() {
    //   this.show = !this.show
    //     },
    products() {
      alert("Alert");
    },
    write() {
      alert("Alert");
    },
    finish() {
      alert("Alert");
    },
  },
};
</script>

<style scoped>
#btn {
  width: 100%;
  height: 20px;
}
#lorem {
  text-decoration: underline greenyellow;
}
button {
  margin-right: 21px;
}
</style>
