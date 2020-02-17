<template>
<div class="col-sm-4">
     <div class="team-member">
       <img class="mx-auto rounded-circle" v-bind:src="imagepath +item.imageURL" alt="">
       <h4>{{item.name}} {{item.surname}}</h4>
       <p class="text-muted">{{item.tag}}</p>
       <ul class="list-inline social-buttons">
         <li class="list-inline-item">
           <a :href="item.socialMedia.tw">
             <i class="fab fa-twitter"></i>
           </a>
         </li>
         <li class="list-inline-item">
           <a :href="item.socialMedia.fb">
             <i class="fab fa-facebook-f"></i>
           </a>
         </li>
         <li class="list-inline-item">
           <a :href="item.socialMedia.in">
             <i class="fab fa-linkedin-in"></i>
           </a>
         </li>
       </ul>
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
        imagepath:"assets/img/team/",
      }
    }
}
</script>

<style>

</style>