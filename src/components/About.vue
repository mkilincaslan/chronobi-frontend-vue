<template>
  <!-- About -->
  <section class="page-section" id="about">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">HAKKIMIZDA</h2>
          <h3 class="section-subheading text-muted">Çalışmalarımız...</h3>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12">
          <ul class="timeline">
            <app-About-Card v-for="item in items" v-bind:key='item.id' v-bind:item="item"/>
            <li class="timeline-inverted">
              <div class="timeline-image">
                <h4>Serüven
                  <br>Yeni
                  <br>Başlıyor!</h4>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import AboutCard from "./AboutCard";
export default {
props:{
  items:{
    type:Array,
    required:true
  }
},
components:{
  appAboutCard:AboutCard
}
}
</script>

<style>

</style>