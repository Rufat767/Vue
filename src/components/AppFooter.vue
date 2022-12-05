<template>
  <div class="container">

<hr>
    <form class="py-3" @submit.prevent="send" action="#">
      Write Somesing:	&#9997;
      <input type="text" v-model="text">
    </form>
    <h5><span class="badge bg-dark">{{text}}</span></h5>
<br>

<hr >
    <p class="text-center py-3 text-warning">
      <span class="badge rounded-pill text-bg-warning width-33px">Vue Js Finish</span>
      <a href="#finish"></a>
    </p>
  </div>
</template>


<script>
export default {
  data(){
    return{
      text : " "
    }

  },
  methods: {
    send(){
      console.log(this.text);
    }
  },
}
</script>
