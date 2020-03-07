<template>
  <!-- Footer -->
  <footer class="footer">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-md-4">
          <span class="copyright">Copyright &copy; Your Website 2019</span>
        </div>
        <div class="col-md-4">
          <app-social-buttons :item="item" />
        </div>
        <div class="col-md-4">
          <ul class="list-inline quicklinks">
            <li class="list-inline-item">
              <a href="/privacy">Privacy Policy</a>
            </li>
            <li class="list-inline-item">
              <a href="/term-of-use">Terms of Use</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
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
components:{
  appSocialButtons:SocialButtons}
}
</script>

<style>

</style>