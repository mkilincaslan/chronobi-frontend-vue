<template>
  <ul class="list-inline social-buttons">
            <li class="list-inline-item">
              <a :href="item.tw">
                <i class="fab fa-twitter"></i>
              </a>
            </li>
            <li class="list-inline-item">
              <a :href="item.fb">
                <i class="fab fa-facebook-f"></i>
              </a>
            </li>
            <li class="list-inline-item">
              <a :href="item.ln">
                <i class="fab fa-linkedin-in"></i>
              </a>
            </li>
            <li class="list-inline-item">
              <a :href="item.in">
                <i class="fab fa-instagram"></i>
              </a>
            </li>
          </ul>
</template>

<script>
export default {
props:{
    item:{
        type:Object,
        required:true
    }
}
}
</script>

<style>

</style>