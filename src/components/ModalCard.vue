<template>
  <div class="portfolio-modal modal fade" :id="'portfolioModal'+item.id" tabindex="-1" role="dialog" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="close-modal" data-dismiss="modal">
          <div class="lr">
            <div class="rl"></div>
          </div>
        </div>
        <div class="container">
          <div class="row">
            <div class="col-lg-8 mx-auto">
              <div class="modal-body">
                <!-- Project Details Go Here -->
                <h2 class="text-uppercase">{{item.name}}</h2>
                <p class="item-intro text-muted">{{item.subTitle}}</p>
                <img class="img-fluid d-block mx-auto" :src="'assets/img/portfolio/'+item.imageURL" alt="">
                <p>{{item.description}}</p>
                <ul class="list-inline">
                  <li>Date: {{item.date}}</li>
                  <li>Client:{{item.client}}</li>
                  <li>Category:{{item.category}}</li>
                </ul>
                <button class="btn btn-primary" data-dismiss="modal" type="button">
                  <i class="fas fa-times"></i>
                  Close Project</button>
              </div>
            </div>
          </div>
        </div>
      </div>
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
}
}
</script>

<style>

</style>