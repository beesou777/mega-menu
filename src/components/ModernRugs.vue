<template>
  <div class="mega-menu-wrapper" v-if="modern_rugs">
    <div class="mega-menu">
      <div class="row">
        <div class="col-md-3 col-sm-12 side-line">
          <ul>
            <li @click="setActiveLink('all_modern_rugs')">
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>See all modern Rugs</span>
              </a>
            </li>
            <li
              @click="setActiveLink('trendy_rugs')"
              :class="{ 'active-link': trendy_rugs }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
              >
                <span>Trendy Rugs</span>
                <svg
                  width="8"
                  height="12"
                  viewBox="0 0 8 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M1.5 1L6.5 6L1.5 11"
                    stroke="#212529"
                    stroke-opacity="0.4"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </a>
            </li>
            <li
              @click="setActiveLink('shop_by_shape')"
              :class="{ 'active-link': shop_by_shape }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>Shop by Shape</span>
                <svg
                  width="8"
                  height="12"
                  viewBox="0 0 8 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M1.5 1L6.5 6L1.5 11"
                    stroke="#212529"
                    stroke-opacity="0.4"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </a>
            </li>
            <li
              @click="setActiveLink('shop_by_color')"
              :class="{ 'active-link': shop_by_color }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>Shop by color</span>
                <svg
                  width="8"
                  height="12"
                  viewBox="0 0 8 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M1.5 1L6.5 6L1.5 11"
                    stroke="#212529"
                    stroke-opacity="0.4"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </a>
            </li>
            <li
              @click="setActiveLink('shop_accessories')"
              :class="{ 'active-link': shop_accessories }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>Shop Accessories</span>
                <svg
                  width="8"
                  height="12"
                  viewBox="0 0 8 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M1.5 1L6.5 6L1.5 11"
                    stroke="#212529"
                    stroke-opacity="0.4"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </a>
            </li>
          </ul>
        </div>
        <div class="col-md-9 col-sm-12">
          <div class="all-modern-rugs bg-light" v-if="all_modern_rugs">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">All Modern Rugs</p>
              </globalNav>
              <a href="#" class="d-flex align-items-center d-none d-md-block">
                <span class="px-3">See all</span>
                <svg
                  width="16"
                  height="16"
                  viewBox="0 0 16 16"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M5.52729 3.52729C5.78764 3.26694 6.20975 3.26694 6.4701 3.52729L10.4701 7.52729C10.7305 7.78764 10.7305 8.20975 10.4701 8.4701L6.4701 12.4701C6.20975 12.7305 5.78764 12.7305 5.52729 12.4701C5.26694 12.2098 5.26694 11.7876 5.52729 11.5273L9.05589 7.9987L5.52729 4.4701C5.26694 4.20975 5.26694 3.78764 5.52729 3.52729Z"
                    fill="#4B6DE2"
                  />
                </svg>
              </a>
            </div>
            <div class="all-rugs-points row justify-content-center">
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
              <div class="col-lg-2 col-md-3 col-sm-12">
                <a href="#">designer tippeche</a>
              </div>
            </div>
          </div>

          <div class="trendy-rugs py-3 bg-light" v-if="trendy_rugs">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">Tredy Rugs</p>
              </globalNav>
              <a href="#" class="d-flex align-items-center d-none d-md-block">
                <span class="px-3">See all</span>
                <svg
                  width="16"
                  height="16"
                  viewBox="0 0 16 16"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M5.52729 3.52729C5.78764 3.26694 6.20975 3.26694 6.4701 3.52729L10.4701 7.52729C10.7305 7.78764 10.7305 8.20975 10.4701 8.4701L6.4701 12.4701C6.20975 12.7305 5.78764 12.7305 5.52729 12.4701C5.26694 12.2098 5.26694 11.7876 5.52729 11.5273L9.05589 7.9987L5.52729 4.4701C5.26694 4.20975 5.26694 3.78764 5.52729 3.52729Z"
                    fill="#4B6DE2"
                  />
                </svg>
              </a>
            </div>
            <div class="trendy-rugs d-flex">
              <div class="d-flex flex-wrap gap-5">
                <div class="sellers-point">
                  <div class="image-wrapper">
                    <img src="../assets/allRugs-1.png" alt="" />
                  </div>
                  <p class="small">All Rugs</p>
                </div>
                <div class="sellers-point">
                  <div class="image-wrapper">
                    <img src="../assets/allRugs-2.png" alt="" />
                  </div>
                  <p class="small">All Rugs</p>
                </div>
                <div class="sellers-point">
                  <div class="image-wrapper">
                    <img src="../assets/allRugs-3.png" alt="" />
                  </div>
                  <p class="small">All Rugs</p>
                </div>
                <div class="sellers-point">
                  <div class="image-wrapper">
                    <img src="../assets/allRugs-4.png" alt="" />
                  </div>
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="sellers-point">
                <div class="image-wrapper">
                  <img src="../assets/top-selling-rugs.png" alt="" />
                </div>
                <p class="small">All Rugs</p>
              </div>
            </div>
          </div>

          <div class="shop-by-shape py-3 bg-light" v-if="shop_by_shape">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">shop by shape</p>
              </globalNav>
            </div>
            <div
              class="container-points d-flex gap-3 align-items-center flex-wrap justify-content-center justify-content-md-start"
            >
              <div class="image-wrapper">
                <img src="../assets/sizes-1.png" alt="" />
                <p class="small">All Rugs</p>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-2.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-3.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-4.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-5.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-5.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
            </div>
          </div>

          <div class="shop-by-color py-3 bg-light" v-if="shop_by_color">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">Shop by color</p>
              </globalNav>
            </div>
            <div
              class="container-points d-flex gap-3 align-items-center flex-wrap justify-content-center justify-content-md-start"
            >
              <div class="image-wrapper">
                <img src="../assets/sizes-1.png" alt="" />
                <p class="small">All Rugs</p>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-2.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-3.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-4.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-5.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/sizes-5.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
            </div>
          </div>

          <div class="shop-accessories py-3 bg-light" v-if="shop_accessories">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">Shop Accessories</p>
              </globalNav>
            </div>
            <div
              class="container-points d-flex gap-3 align-items-center flex-wrap justify-content-center justify-content-md-start"
            >
              <div class="image-wrapper">
                <img src="../assets/shape-1.png" alt="" />
                <p class="small">All Rugs</p>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/shape-2.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/shape-3.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/shape-4.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/shape-5.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/shape-5.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
    
<script>
import globalNav from './globalNav.vue';
export default {
  props: {
    modern_rugs: {
      type: Boolean,
      default: true,
    },
  },
  data() {
    return {
      all_modern_rugs: true,
      trendy_rugs: false,
      shop_by_shape: false,
      shop_by_color: false,
      shop_accessories: false,
    };
  },
  components:{
    globalNav
  },  
  methods: {
    setActiveLink(link) {
      this.all_modern_rugs = link === "all_modern_rugs";
      this.trendy_rugs = link === "trendy_rugs";
      this.shop_by_shape = link === "shop_by_shape";
      this.shop_by_color = link === "shop_by_color";
      this.shop_accessories = link === "shop_accessories";
    },
    backButton() {
      this.all_modern_rugs = false;
      this.trendy_rugs = false;
      this.shop_accessories = false;
      this.shop_by_shape = false;
      this.shop_by_color = false;
    },
  },
  mounted() {
    const windowSize = window.innerWidth;
    if (windowSize <= 767) {
      this.all_modern_rugs = false;
    }
  },
};
</script>
    