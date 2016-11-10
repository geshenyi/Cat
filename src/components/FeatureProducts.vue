<template>
  <div class="pure-g full-width feature-products-section">
    <div class="pure-u-1">
      <div class="section-label">
        FEATURE PRODUCTS
      </div>
    </div>
    <div class="pure-u-1">
      <div class="pure-g">
        <div class="pure-u-1-2 pure-u-md-1-4 pure-u-lg-1-4" v-for="product in products">
          <div class="img-wrapper">
            <img v-bind:src="product.imgUrl" class="full-width"/>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.section-label{
  text-align: center;
  font-size: 3rem;
  color: #8e8888;
}
.feature-products-section{
  margin-top: 50px;
}
.img-wrapper{
  padding: 5px;
}
</style>

<script>
    export default{
        name: "FeatureProducts",
        data(){
            return{
                msg:'hello vue',
                products:[
                  {
                    imgUrl: "/static/images/2.jpg"
                  },
                  {
                    imgUrl: "/static/images/3.jpg"
                  },
                  {
                    imgUrl: "/static/images/4.jpg"
                  },
                  {
                    imgUrl: "/static/images/5.jpg"
                  },
                ]
            }
        },
        components:{

        },
        beforeMount(){
        }
    }



</script>
