<template>
      <div class="col-md-4">
      <span class="fa-stack fa-4x">
        <i class="fas fa-circle fa-stack-2x text-primary"></i>
        <i :class="item.icon"></i>
      </span>
      <h4 class="service-heading">{{item.name}}</h4>
      <p class="text-muted">{{item.description}}</p>
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
        
      }
    }
}
</script>

<style>

</style>