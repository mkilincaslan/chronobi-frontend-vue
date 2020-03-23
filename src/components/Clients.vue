<template>
  <!-- Clients -->
  <section class="py-5">
    <div class="container">
      <div class="text-center"><h3 style="">Sponsorluklar</h3></div>
      <div class="row">
        <app-client-card v-for="item in items" v-bind:key='item.id' v-bind:item="item"/>
      </div>
    </div>
  </section>
</template>

<script>
import ClientCard from "./ClientCard";
export default {
props:{
  items:{
    type:Array,
    required:true
  }
},
components:{
  appClientCard:ClientCard
}
}
</script>

<style>

</style>