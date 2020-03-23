<template>
  <!-- Team -->
  <section class="bg-light page-section" id="team">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">TAKIM ÜYELERİ</h2>
          <h3 class="section-subheading text-muted">Kurucu Üyeler</h3>
        </div>
      </div>
      <div class="row">
              <app-team-card v-for="item in items" v-bind:key='item.id' v-bind:item="item"/>
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