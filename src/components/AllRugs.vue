<template>
  <div class="mega-menu-wrapper" v-if="all_rugs">
    <div class="mega-menu">
      <div class="row">
        <div class="col-md-3 col-sm-12 side-line">
          <ul>
            <li @click="setActiveLink('see_all_rugs')">
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>Sell all rugs</span>
              </a>
            </li>
            <li
              @click="setActiveLink('top_seller')"
              :class="{ 'active-link': top_seller }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>Top Sellers</span>
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
              @click="setActiveLink('new_arrivals')"
              :class="{ 'active-link': new_arrivals }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>New Arrivals</span>
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
              @click="setActiveLink('shop_by_size')"
              :class="{ 'active-link': shop_by_size }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>Shop by Size</span>
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
                ><span>Shop by shape</span>
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
              @click="setActiveLink('shop_by_room')"
              :class="{ 'active-link': shop_by_room }"
            >
              <a
                href="#"
                class="d-flex align-items-center justify-content-between"
                ><span>Shop by Room</span>
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
          <div class="see-all-rugs bg-light" v-if="see_all_rugs">
            <div class="bars gap-3 align-items-center ">
            <globalNav>
              <p class="back-button" @click="backButton">back</p>
            <p class="text">Top Sellers</p>
            </globalNav>
              <a href="#" class="d-flex align-items- d-md-block d-none">
                <span class="px-3">See all Rugs</span>
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
            <div class="all-rugs-points d-flex align-items-center">
              <div class="rugs-container">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-1.png" alt="" />
                </div>
                <p class="small">All Rugs</p>
              </div>

              <div class="rugs-container">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-2.png" alt="" />
                </div>
                <p class="small">All Rugs</p>
              </div>

              <div class="rugs-container">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-3.png" alt="" />
                </div>
                <p class="small">All Rugs</p>
              </div>

              <div class="rugs-container">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-4.png" alt="" />
                </div>
                <p class="small">All Rugs</p>
              </div>

              <div class="rugs-container">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-5.png" alt="" />
                </div>
                <p class="small">All Rugs</p>
              </div>
            </div>
          </div>

          <div class="top-sellers py-3 bg-light" v-if="top_seller">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">Top Sellers</p>
              </globalNav>
              <a href="#" class="d-flex align-items-center">
                <span class="px-3">See all Rugs</span>
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
            <div class="top-seller-points d-flex">
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

          <div class="new-arrivals py-3 bg-light" v-if="new_arrivals">
            <div class="bars">
             <globalNav>
              <p class="back-button" @click="backButton">back</p>
              <p class="text">New Arrival</p>
             </globalNav>
              <p class="head-3 mb-0">Rugs</p>
              <a href="#" class="d-flex align-items-center">
                <span class="px-3">See all Rugs</span>
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
            <div class="container-points d-flex">
              <div class="d-flex flex-wrap gap-5">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-1.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
                <div class="image-wrapper">
                  <img src="../assets/allRugs-2.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
                <div class="image-wrapper">
                  <img src="../assets/allRugs-3.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
                <div class="image-wrapper">
                  <img src="../assets/allRugs-4.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="image-wrapper">
                <img src="../assets/top-selling-rugs.png" alt="" />
                <p class="small">All Rugs</p>
              </div>
            </div>
          </div>

          <div class="shop-by-size py-3 bg-light" v-if="shop_by_size">
            <div class="bars">
             <globalNav>
              <p class="back-button" @click="backButton">back</p>
              <p class="text">Shop By Size</p>
             </globalNav>
              <p class="head-3 mb-0">shape</p>
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

          <div class="shop-by-shape py-3 bg-light" v-if="shop_by_shape">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">Shop by Shape</p>
              </globalNav>
              <p class="head-3 mb-0">Sizes</p>
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

          <div class="shop-by-color py-3 bg-light" v-if="shop_by_color">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">Shop by color</p>
              </globalNav>
              <p class="head-3 mb-0">Rugs</p>
              <a href="#" class="d-flex align-items-center">
                <span class="px-3">See all Rugs</span>
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
            <div class="container-points d-flex gap-3 align-items-center">
              <div class="image-wrapper">
                <img src="../assets/allRugs-1.png" alt="" />
                <p class="small">All Rugs</p>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-2.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-3.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-4.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/allRugs-5.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
            </div>
          </div>

          <div class="shop-by-room py-3 bg-light" v-if="shop_by_room">
            <div class="bars">
              <globalNav>
                <p class="back-button" @click="backButton">back</p>
                <p class="text">Shop by Room</p>
              </globalNav>
              <p class="head-3 mb-0">Rooms</p>
              <a href="#" class="d-flex align-items-center">
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
            <div
              class="container-points d-flex gap-3 align-items-center justify-content-around justify-content-md-auto"
            >
              <div class="image-wrapper">
                <img src="../assets/room-1.png" alt="" />
                <p class="small">All Rugs</p>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/room-2.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/room-3.png" alt="" />
                  <p class="small">All Rugs</p>
                </div>
              </div>
              <div class="category-container py-3">
                <div class="image-wrapper">
                  <img src="../assets/room-4.png" alt="" />
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
    all_rugs: {
      type: Boolean,
      default:true
    },
    title:{
      type:String
    },
    backButton:{
      type:Function
    }
  },
  data() {
    return {
      see_all_rugs: true,
      top_seller: false,
      new_arrivals: false,
      shop_by_size: false,
      shop_by_shape: false,
      shop_by_color: false,
      shop_by_room: false,
    };
  },
components:{
  globalNav
},
  methods: {
    setActiveLink(link) {
      this.see_all_rugs = link === "see_all_rugs";
      this.top_seller = link === "top_seller";
      this.new_arrivals = link === "new_arrivals";
      this.shop_by_size = link === "shop_by_size";
      this.shop_by_shape = link === "shop_by_shape";
      this.shop_by_color = link === "shop_by_color";
      this.shop_by_room = link === "shop_by_room";
    },
    backButton() {
      this.see_all_rugs = false;
      this.top_seller = false;
      this.new_arrivals = false;
      this.shop_by_size = false;
      this.shop_by_shape = false;
      this.shop_by_color = false;
      this.shop_by_room = false;
    },


  },
  mounted() {
    const windowSize = window.innerWidth;
    if (windowSize <= 767) {
      this.see_all_rugs = false;
    }
  },
};
</script>
  