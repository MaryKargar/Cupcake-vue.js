!<template>
<div class="row">
    <div v-for="(cake,index) in cakes" :key="index" class="card" style="width: 18rem;">
  <img :src="getImg(cake.img)" class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">{{cake.title}}</h5>
    <p class="card-text">eggs, milk, oil, and vanilla</p>
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Ingredients</li>
    <li class="list-group-item">Topping</li>
    <li class="list-group-item">Time</li>
  </ul>
  <div class="card-body">
    <a href="https://www.gutekueche.at/schoko-cupcake-rezept-5032" class="card-link">www.gutekueche.at</a>
    <a href="https://www.einfachbacken.de/rezepte/schoko-cupcakes" class="card-link">www.einfachbacken.de</a>
  </div>
</div>
</div>
  
</template>

<script>
import 'bootstrap';
import 'bootstrap/dist/css/bootstrap.min.css'
export default {
props:['cakes'],
methods: {
  getImg(img) { return require('@/assets/' + img) }
  }
}

</script>

<style>

</style>