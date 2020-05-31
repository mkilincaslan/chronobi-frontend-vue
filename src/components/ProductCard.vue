<template>
      <div class="col-md-4 col-sm-6 portfolio-item">
      <a class="portfolio-link text-center" data-toggle="modal" :value="item.id" :href="'#portfolioModal'+item.id">
        <div class="portfolio-hover">
          <div class="portfolio-hover-content text-center">
            <i class="fas fa-plus fa-3x"></i>
          </div>
        </div>
        <img class="img-fluid img-responsive" style="max-width: 100%; height: auto;" v-bind:src="imagepath +item.imageURL" v-bind:alt='item.imageURL'>
      </a>
      <div class="portfolio-caption">
        <h4>{{item.name}}</h4>
        <p class="text-muted">{{item.subTitle}}</p>
      </div>
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