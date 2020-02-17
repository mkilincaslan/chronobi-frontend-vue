<template>
  <!-- Team -->
  <section class="bg-light page-section" id="team">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Our Amazing Team</h2>
          <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
        </div>
      </div>
      <div class="row">
              <app-team-card v-for="item in items" v-bind:key='item.id' v-bind:item="item"/>
      </div>
      <div class="row">
        <div class="col-lg-8 mx-auto text-center">
          <p class="large text-muted">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut eaque, laboriosam veritatis, quos non quis ad perspiciatis, totam corporis ea, alias ut unde.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import TeamCard from "./TeamCard";
export default {
props:{
  items:{
    type:Array,
    required:true
  }
},
components:{
  appTeamCard:TeamCard
}
}
</script>

<style>

</style>