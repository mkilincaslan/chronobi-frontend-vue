<template>
  <!-- Services -->
  <section class="page-section" id="services">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Services</h2>
          <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
        </div>
      </div>
      <div class="row text-center">
        <app-service-card v-for="item in items" v-bind:key='item' v-bind:item="item"/>
      </div>
    </div>
  </section>
</template>

<script>
import ServiceCard from "./ServiceCard";
export default {
props:{
  items:{
    type:Array,
    required:true
  }
},
components:{
  appServiceCard:ServiceCard
}
}
</script>

<style>

</style>