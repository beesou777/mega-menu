<template>
    <div class="mega-menu-wrapper" v-if="sales">
      <div class="mega-menu">
        <div class="row p-3">
            <div class="col-lg-3 col-md-4 col-sm-12">
                <div class="sale-content">
                    <div class="img-wrapper">
                        <img src="../assets/top-selling-rugs.png" alt="sale" class="w-100">
                    </div>
                </div>
            </div>
            <div class="col-lg-3 col-md-4 col-sm-12">
                <div class="sale-content">
                    <div class="img-wrapper">
                        <img src="../assets/top-selling-rugs.png" alt="sale" class="w-100">
                    </div>
                </div>
            </div>
            <div class="col-lg-3 col-md-4 col-sm-12">
                <div class="sale-content">
                    <div class="img-wrapper">
                        <img src="../assets/top-selling-rugs.png" alt="sale" class="w-100">
                    </div>
                </div>
            </div>
            <div class="col-lg-3 col-md-4 col-sm-12">
                <div class="sale-content">
                    <div class="img-wrapper">
                        <img src="../assets/top-selling-rugs.png" alt="sale" class="w-100">
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
      sales: {
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
    