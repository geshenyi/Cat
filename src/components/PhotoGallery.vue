<template>
  <div class="pure-g full-width feature-products-section">
    <div class="pure-u-1">
      <div class="section-label">
        PHOTO GALLERY
      </div>
    </div>
    <div class="pure-u-1 pure-u-md-1-3 pure-u-lg-1-3 main-image-section">
      <div class="main-image-wrapper">
        <img v-bind:src="mainImage" class="full-width full-height"/>
      </div>
    </div>
    <div class="pure-u-1 pure-u-md-2-3 pure-u-lg-2-3">
      <div class="pure-g">
        <div class="pure-u-1-2 pure-u-md-1-3 pure-u-lg-1-3" v-for="photo in photos">
          <div class="small-photo-wrapper">
            <img v-bind:src="photo.imgUrl" class="full-width small-photo"/>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.small-photo{
 height: 100%;
}

.main-image-section {
  padding-bottom: 4px;
}

.main-image-wrapper{
  height: 100%;
}

.small-photo-wrapper{
  padding: 0 1px 0 1px;
}

.small-photo-wrapper:hover{
  -webkit-filter: opacity(.7);
  filter: opacity(.7);
}

</style>

<script>
    export default{
        name: "PhotoGallery",
        data(){
            return{
                msg:'hello vue',
                mainImage: "/static/images/repo.png",
                photos:[
                  {
                    imgUrl: "/static/images/6.jpg"
                  },
                  {
                    imgUrl: "/static/images/7.jpg"
                  },
                  {
                    imgUrl: "/static/images/8.jpg"
                  },
                  {
                    imgUrl: "/static/images/9.jpg"
                  },
                  {
                    imgUrl: "/static/images/10.jpg"
                  },
                  {
                    imgUrl: "/static/images/11.jpg"
                  },
                  {
                    imgUrl: "/static/images/12.jpg"
                  },
                  {
                    imgUrl: "/static/images/13.jpg"
                  },
                  {
                    imgUrl: "/static/images/14.jpg"
                  },
                ]
            }
        },
        components:{
        }
    }






</script>
