<template>
              <li>
              <div class="timeline-image">
                <img class="rounded-circle img-fluid" :src="imagepath + item.imageURL" alt="">
              </div>
              <div class="timeline-panel">
                <div class="timeline-heading">
                  <h4>{{item.date}}</h4>
                  <h4 class="subheading">{{item.title}}</h4>
                </div>
                <div class="timeline-body">
                  <p class="text-muted">{{item.description}}</p>
                </div>
              </div>
            </li>
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
        imagepath:"assets/img/about/",
      }
    }
}
</script>

<style>

</style>