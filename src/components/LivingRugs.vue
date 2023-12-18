<template>
    <div class="mega-menu-wrapper" v-if="living_rugs">
      <div class="mega-menu">
        <div class="row p-0 p-md-3">
          <div class="col-lg-8 col-md-6 col-sm-12">
            <p class="head-3 d-none d-md-block">living rugs</p>
            <div class="row">
              <div class="col-md-4 col-lg-3 col-6">
                <div class="living-content">
                  <div class="img-wrapper">
                    <img src="../assets/room-1.png" alt="living rugs" class="w-100">
                  </div>
                  <p class="small">vintage</p>
                </div>
              </div>
              <div class="col-md-4 col-lg-3 col-6">
                <div class="living-content">
                  <div class="img-wrapper">
                    <img src="../assets/room-1.png" alt="living rugs" class="w-100">
                  </div>
                  <p class="small">vintage</p>
                </div>
              </div>
              <div class="col-md-4 col-lg-3 col-6">
                <div class="living-content">
                  <div class="img-wrapper">
                    <img src="../assets/room-1.png" alt="living rugs" class="w-100">
                  </div>
                  <p class="small">vintage</p>
                </div>
              </div>
              <div class="col-md-4 col-lg-3 col-6">
                <div class="living-content">
                  <div class="img-wrapper">
                    <img src="../assets/room-1.png" alt="living rugs" class="w-100">
                  </div>
                  <p class="small">vintage</p>
                </div>
              </div>
              <div class="col-md-4 col-lg-3 col-6">
                <div class="living-content">
                  <div class="img-wrapper">
                    <img src="../assets/room-1.png" alt="living rugs" class="w-100">
                  </div>
                  <p class="small">vintage</p>
                </div>
              </div>
              <div class="col-md-4 col-lg-3 col-6">
                <div class="living-content">
                  <div class="img-wrapper">
                    <img src="../assets/room-1.png" alt="living rugs" class="w-100">
                  </div>
                  <p class="small">vintage</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 col-sm-12 d-none d-md-block">
            <div class="content-wrapper">
              <div class="img-wrapper">
                <img src="../assets/top-selling-rugs.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
    
  <script>
  export default {
    props: {
      living_rugs: {
        type: Boolean,
        default:true
      },
    },
    data() {
      return {
      };
    },
  
    methods: {
    },
  };
  </script>
    