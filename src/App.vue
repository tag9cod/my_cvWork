<template>
  <div class="container" style="background-color: rgb(97, 21, 130);">
      <div class="row g-5">
          <sideBar/>
          <div class="col-lg-8" style="background-color: rgb(103, 24, 137);">
              <mainBar/>
              <Foot/>
          </div>
      </div>
  </div>
   <!-- Back to Top -->
   <a href="#" class="back-to-top"><i class="fa fa-angle-double-up"></i></a>
</template>

<script>
import sideBar from './components/sideBar.vue'
import mainBar from './components/mainBar.vue'
import Foot from './components/FooTer.vue'
export default {
  name : 'App',
  components: {
    sideBar,
    mainBar,
    Foot
  }
}
</script>
