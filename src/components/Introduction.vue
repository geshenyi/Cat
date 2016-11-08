<template>
  <div class="pure-g full-width feature-products-section">
    <div class="pure-u-1">
      <div class="section-label">
        Ancient Tree Introduction
      </div>
    </div>
    <div class="pure-u-1-3" v-for="intro in intros">
      <div class="pure-g intro-wrapper">
        <div class="pure-u-1">
          <img v-bind:src="intro.imgUrl" class="full-width intro-image"/>
        </div>
        <div class="pure-u-1 intro-text">
            But the long, unusual and often ugly 2016 presidential campaign has been about the country’s changing demographics and the shifting coalitions of the two major parties as much as about the two main candidates.

Trump expresses confidence while criticizing the media and public polls.

As the polls opened on Tuesday morning, Mr. Trump said he would do “very well” in the crucial battleground states of Florida, North Carolina and Ohio, and acknowledged that after nearly a year and a half of campaigning the only thing left for him to do was wait and see.
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.intro-wrapper{
  padding: 50px;
}

.intro-image{
  height: 130px;
}

.intro-text{
  text-align: left;
  line-height: 30px;
}

</style>

<script>
    export default{
        name: "Introduction",
        data(){
            return{
                msg:'hello vue',
                intros: [
                  {
                    imgUrl: "/static/images/logo1.png"
                  },
                  {
                    imgUrl: "/static/images/logo2.png"
                  },
                  {
                    imgUrl: "/static/images/logo3.png"
                  }
                ]
            }
        },
        components:{
        }
    }







</script>
