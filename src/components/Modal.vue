<template>
  <div>
    <app-modal-card v-for="item in items" v-bind:key='item.id' v-bind:item="item" />
  </div>
</template>

<script>
import ModalCard from "./ModalCard";
export default {
 components:{
   appModalCard:ModalCard
 } ,
props:{
  items:{
    type:Array,
    required:true
  }
}
}
</script>

<style>

</style>