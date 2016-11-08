<template>
  <div id="app" class="pure-g">
    <global-header></global-header>
    <div class="pure-u-1">
      <img src="./assets/1.jpg" id="main-image">
    </div>
    <feature-products></feature-products>
    <photo-gallery></photo-gallery>
    <introduction></introduction>
    <carousel>
      <slider>
        <img src="https://placehold.it/1200x500?text=one">
        <div class="carousel-caption">
          <h3>Slide #1</h3>
          <p>sunt in culpa qui officia deserunt mollit a.</p>
        </div>
      </slider>
      <slider>
        <img src="https://placehold.it/1200x500?text=two">
        <div class="carousel-caption">
          <h3>Slide #2</h3>
          <p>sunt in culpa qui officia deserunt mollit a.</p>
        </div>
      </slider>
      <slider>
        <img src="https://placehold.it/1200x500?text=three">
        <div class="carousel-caption">
          <h3>Slide #3</h3>
          <p>sunt in culpa qui officia deserunt mollit a.</p>
        </div>
      </slider>
    </carousel>
  </div>
</template>

<script>
import GlobalHeader from './components/GlobalHeader'
import FeatureProducts from './components/FeatureProducts'
import PhotoGallery from './components/PhotoGallery'
import Introduction from './components/Introduction'
import carousel from './vue-strap/src/carousel'
import slider from './vue-strap/src/Slider.vue'
import bootstrap from './bootstrap/dist/css/bootstrap.css'

export default {
  name: 'app',
  components: {
    GlobalHeader, FeatureProducts,PhotoGallery,Introduction, carousel, slider
  }
}

</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#main-image{
  width: 100%;
}

body{
  margin: 0px;
}

.full-height{
  height: 100%;
}

.full-width{
  width: 100%;
}

</style>
