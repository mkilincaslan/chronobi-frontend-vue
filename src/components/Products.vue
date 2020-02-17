<template>
  <!-- Portfolio Grid -->
  <section class="bg-light page-section" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Portfolio</h2>
          <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
        </div>
      </div>
      <div class="row">
        <app-Product-Card v-for="item in items" v-bind:key='item' v-bind:item="item"/>
      </div>
    </div>
  </section>
</template>

<script>
import ProductCard from "./ProductCard";
export default {
props:{
  items:{
    type:Array,
    required:true
  }
},
components:{
  appProductCard:ProductCard
}
}
</script>

<style>

</style>