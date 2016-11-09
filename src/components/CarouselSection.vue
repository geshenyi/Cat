<template>
  <div class="pure-g full-width carousel-wrapper">
    <div class="pure-u-1 full-height">
      <div class="carousel-hook pure-g">
        <div class="item-wrapper pure-u-1" v-for="banner in banners">
          <div class="position-relative">
            <div class="item-caption">
              {{banner.content}}
            </div>
            <img v-bind:src="banner.imgUrl" class="banner-image"/>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.carousel-wrapper{

}
.carousel-image {
  width: 100%;
  height: 400px;
}

.item-wrapper{
  text-align: center;
}

.your-class{
  padding: 10px;
}

.item-caption{
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.62);
  padding-top: 15%;
  font-size: 4rem;
  color: white;
}

.banner-image{
  max-width: 100%;
  height: 100%;
}


</style>

<script>
    import carousel from '../vue-strap/src/Carousel.vue'
    import slider from '../vue-strap/src/Slider.vue'
    import bootstrap from '../bootstrap/dist/css/bootstrap.css'
    import $ from 'jquery'
    import 'slick-carousel'
    import slickCss from '../slick/slick.css'
    import slickTheme from '../slick/slick-theme.css'
    export default{
        name: 'CarouselSection',
        data(){
            return{
                banners:[
                  {
                    content: 'New Product Launch',
                    imgUrl: 'http://www.inovit.com/images/index/newsBanner1.jpg'
                  },
                  {
                    content: 'Love This Fancy Car?',
                    imgUrl: 'http://www.inovit.com/images/index/newsBanner2.jpg'
                  },
                  {
                    content: 'Rock it!!!',
                    imgUrl: 'http://www.inovit.com/images/index/newsBanner3.jpg'
                  }
                ]
            }
        },
        components:{
          carousel, slider,
        },
        methods: {
          next() {
              this.$refs.slick.next();
          },
          prev() {
              this.$refs.slick.prev();
          }
        },
        mounted(){
          $('.carousel-hook').slick({
            dots: false,
            autoplay: true,
            arrows: false,
            infinite: true,
            autoplaySpeed: 2000
          });
        }
    }




</script>
