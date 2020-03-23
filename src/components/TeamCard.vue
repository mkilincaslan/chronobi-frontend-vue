<template>
<div class="col-sm-4">
     <div class="team-member">
       <img class="mx-auto rounded-circle" v-bind:src="imagepath +item.imageURL" alt="">
       <h4>{{item.name}} {{item.surname}}</h4>
       <p class="text-muted">{{item.tag}}</p>
       <app-social-buttons :item="item.socialMedia" />
     </div>
   </div>
</template>

<script>
import SocialButtons from "./SocialButtons";
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
    },
    components:{
      appSocialButtons:SocialButtons
    }

}
</script>

<style>

</style>