<template>
  <div id="app" class="pure-g">
    <global-header></global-header>
    <div class="pure-u-1">
      <img src="./assets/1.jpg" id="main-image">
    </div>
    <feature-products></feature-products>
    <photo-gallery></photo-gallery>
    <introduction></introduction>
    <carousel-section></carousel-section>
    <welcome-section></welcome-section>
  </div>
</template>

<script>
import GlobalHeader from './components/GlobalHeader'
import FeatureProducts from './components/FeatureProducts'
import PhotoGallery from './components/PhotoGallery'
import Introduction from './components/Introduction'
import CarouselSection from './components/CarouselSection'
import WelcomeSection from './components/WelcomeSection'

export default {
  name: 'app',
  components: {
    GlobalHeader, FeatureProducts,PhotoGallery,Introduction, CarouselSection, WelcomeSection
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

.position-relative{
  position: relative;
}
</style>
