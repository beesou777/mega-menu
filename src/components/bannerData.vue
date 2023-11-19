<template>
    <div class="banner-content p-3">
      <p class="head-2 mb-2">{{ title }}</p>
      <p class="body-2 mb-1">{{ sub_title }}</p>
    </div>
    <div class="image-wrapper ">
      <img :src="image" alt="" />
      <div class="button-wrapper">
        <a href="{{ button_link }}"> <button>{{ button_text }}</button></a>
      </div>
    </div>
</template>
<script>
export default {
  props: {
    title:{
        type:String
    },
    sub_title:{
        type:String
    },
    button_text:{
        type:String
    },
    button_link:{
        type:String
    },
    image:{
        type:String
    }
  },

  data() {},
};
</script>
<style lang="sass" scoped>
.banner-container{
    max-height: 300px;
    max-width: 300px;
    width: 100%;
    margin: auto;
    border-radius: 12px;
    overflow: hidden;
    .banner-content{
      background-color: $primary-color;
      p.head-2{
        color: $white;
      }
      p.body-2{
        color: $light-200;
      }
  
    }
    .image-wrapper{
      max-height: 200px;
      max-width: 300px;
      width: 100%;
      height: 200px;
      background: transparent;
      img{
        width: 100%;
        object-fit: contain;
      }
      .button-wrapper{
        transform: translate(6%,-160%);
        button{
          padding: .5rem 1rem;
          border: 0;
          border-radius: 4px;
          color: $primary-color;
          font-weight: 600;
        }
      }
    }
  }
</style>