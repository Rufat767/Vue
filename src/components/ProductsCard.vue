<template>
  <div class="row bg-success">
    <div  class="col-3 py-3"  v-for="(item,index) in 20" :key="(item.id)">
      <div  class="card" style="width: 18rem py-3">
        <div  class="card-body">
          <h5 class="card-title">{{(index+1)}}</h5>
          <h6 class="card-subtitle mb-2 text-muted">fasaf</h6>
          <p class="card-text">
            afasfd
          </p>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  created(){
    fetch('https://fakestoreapi.com/products').then(response => {
      response.json().then(products =>{
        console.log(products); ;
      })
    })
  }
  };
</script>
