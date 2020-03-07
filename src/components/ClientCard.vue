<template>
  <div class="col-md-3 col-sm-6">
          <a :href="item.link">
            <img class="img-fluid d-block mx-auto" v-bind:src="imagepath +item.logo" alt="">
          </a>
  </div>
</template>

<script>

export default {
    props:{
        item:{
            type:Object,
            required:true
        }
    },
    data:function (){
      return {
        imagepath:"assets/img/portfolio/",
      }
    }
}
</script>

<style>

</style>