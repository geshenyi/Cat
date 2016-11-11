<template>
  <div class="pure-g full-width footer-wrapper">
    <div class="pure-u-1-2 pure-u-md-1-4 pure-u-lg-1-4">
      <h4>Products</h4>
      <ul class="footer-list">
        <li>
          Cabinet 1
        </li>
        <li>
          Cabinet 2
        </li>
        <li>
          Cabinet 3
        </li>
      </ul>
    </div>
    <div class="pure-u-1-2 pure-u-md-1-4 pure-u-lg-1-4">
      <h4>About Us</h4>
      <ul class="footer-list">
        <li>
          Careers
        </li>
        <li>
          Communities
        </li>
        <li>
          Contact Us
        </li>
        <li>
          History
        </li>
        <li>
          Partners
        </li>
      </ul>
    </div>
    <div class="pure-u-1-2 pure-u-md-1-4 pure-u-lg-1-4">
      <h4>Branch</h4>
      <ul class="footer-list">
        <li>
          Australia
        </li>
        <li>
          Holland
        </li>
        <li>
          Italy
        </li>
        <li>
          P.R.China
        </li>
        <li>
          United States
        </li>
      </ul>
    </div>
    <div class="pure-u-1-2 pure-u-md-1-4 pure-u-lg-1-4">
      <div class="pure-g">
        <div class="pure-u-1-3"></div>
        <div class="pure-u-1-3" id="social-media-wrapper">
          <h4>Social Media</h4>
          <ul class="footer-list">
            <li>
              <a id="wechat-link">Wechat</a>
            </li>
            <li>
              <a id="facebook-link">Fackbook</a>
            </li>
            <li>
              <a id="twitter-link">Twitter</a>
            </li>
            <li>
              <a id="linkedin-link">LinkedIn</a>
            </li>
          </ul>
        </div>
        <div class="pure-u-1-3"></div>
      </div>
    </div>
    <div class="pure-u-1 full-width foot-info">
      <div class="pure-g">
        <div class="pure-u-1-3">
          @2008-2016 Ancient Tree
        </div>
        <div class="pure-u-1-3">
          Ancient Tree
        </div>
        <div class="pure-u-1-3">
          Have Questions? +86 88888888
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.footer-wrapper{
 background-color: #f6f6f6;
 padding: 80px 100px 30px 100px;
}

.footer-list{
  list-style-type: none;
  padding: 0;
  margin: 0;
  color: #575353;
  line-height: 40px;
}

#wechat-link{
  background: url(/static/images/wechat.jpg) left center no-repeat;
  background-size: 30px 30px;
  padding-left: 35px;
  display: inline-block;
}

#facebook-link{
  background: url(/static/images/facebook.png) left center no-repeat;
  background-size: 30px 30px;
  padding-left: 35px;
  display: inline-block;
}

#twitter-link{
  background: url(/static/images/twitter.png) left center no-repeat;
  background-size: 30px 30px;
  padding-left: 35px;
  display: inline-block;
}

#linkedin-link{
  background: url(/static/images/linkedin.png) left center no-repeat;
  background-size: 30px 30px;
  background-position: px;
  padding-left: 35px;
  display: inline-block;
}

#social-media-wrapper {
  text-align: left;
}

.foot-info{
  margin-top: 50px;
  border-top: 1px solid lightgrey;
}


</style>

<script>
    export default{
        name: 'Footer',
        data(){
            return{
            }
        },
        components:{
        }
    }






</script>
