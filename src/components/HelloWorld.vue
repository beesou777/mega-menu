<template>
  <div class="nav-links border mt-5">
    <div
      class="hamburger-part d-block d-md-none"
      @click="showSmallDeviceComponent = !showSmallDeviceComponent"
    >
      ham
    </div>
    <div class="desktop-link" v-if="!showSmallDeviceComponent">
      <ul class="d-flex gap-3">
        <li @click="setActiveLink('all_rugs')">
          <a href="#">Alle Teppiche</a>
          <all-rugs v-if="all_rugs"/>
        </li>
        <li>
          <a href="#" @click="setActiveLink('modern_rugs')">modern rugs</a>
          <modern-rugs v-if="modern_rugs" />
        </li>
        <li>
          <a href="#" @click="setActiveLink('shop_by_room')">Alle Teppiche</a>
        </li>
        <li>
          <a href="#" @click="setActiveLink('living_rugs')">Living rugs</a>
          <living-rugs v-if="living_rugs" />
        </li>
        <li>
          <a href="#" @click="setActiveLink('shop_by_room')">Blogs</a>
        </li>
        <li>
          <a href="#" @click="setActiveLink('sales')">Sale</a>
          <sale v-if="sales" />
        </li>
      </ul>
    </div>

    <div class="small-device h-100 p-3" v-else>
      <div class="d-flex justify-content-between">
        <p class="close">close</p>
        <p class="logo">logo</p>
      </div>
      <div class="all-rugs my-3">
        <div class="d-flex justify-content-between" @click="all_rugs = !all_rugs">
          <p class="text mb-0">All Rugs</p>
          <svg
            width="20"
            height="21"
            viewBox="0 0 20 21"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g opacity="0.4">
              <path
                d="M9.9974 4.66602V16.3327M4.16406 10.4993H15.8307"
                stroke="black"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </g>
          </svg>
        </div>
        <all-rugs  v-if="all_rugs" />
      </div>
      <div class="modern-rugs my-3">
        <div class="d-flex justify-content-between" @click="modern_rugs = !modern_rugs">
          <p class="text mb-0">Modern Rugs</p>
          <svg
            width="20"
            height="21"
            viewBox="0 0 20 21"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g opacity="0.4">
              <path
                d="M9.9974 4.66602V16.3327M4.16406 10.4993H15.8307"
                stroke="black"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </g>
          </svg>
        </div>
        <modern-rugs v-if="modern_rugs" />
      </div>
      <div class="Oriental-rugs my-3">
        <div class="d-flex justify-content-between">
          <p class="text mb-0">Orienal Rugs</p>
          <svg
            width="20"
            height="21"
            viewBox="0 0 20 21"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g opacity="0.4">
              <path
                d="M9.9974 4.66602V16.3327M4.16406 10.4993H15.8307"
                stroke="black"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </g>
          </svg>
        </div>
        <oriental-rug v-if="oriental_rugs" />
      </div>
      <div class="living-rooms my-3">
        <div class="d-flex justify-content-between" @click="living_rugs = !living_rugs">
          <p class="text mb-0">Living Rooms</p>
          <svg
            width="20"
            height="21"
            viewBox="0 0 20 21"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g opacity="0.4">
              <path
                d="M9.9974 4.66602V16.3327M4.16406 10.4993H15.8307"
                stroke="black"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </g>
          </svg>
        </div>
        <living-rugs v-if="living_rugs"/>
      </div>

    </div>
  </div>
</template>
<script>
import AllRugs from "./AllRugs.vue";
import ModernRugs from "./ModernRugs.vue";
import OrientalRugs from "./OrientalRugs.vue";
import LivingRugs from "./LivingRugs.vue";
import Sale from "./Sale.vue";
export default {
  data() {
    return {
      all_rugs: false,
      modern_rugs: false,
      living_rugs: false,
      oriental_rugs:false,
      sales: false,
      showSmallDeviceComponent: false,
    };
  },
  components: {
    AllRugs,
    ModernRugs,
    LivingRugs,
    Sale,
    OrientalRugs
  },
  methods: {
    setActiveLink(link) {
      this.all_rugs = link === "all_rugs";
      this.modern_rugs = link === "modern_rugs";
      this.oriental_rugs = link === "oriental_rugs";
      this.living_rugs = link === "living_rugs";
      this.sales = link === "sales";
    },
  },
};
</script>
  