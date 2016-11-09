<template>
  <div class="pure-g full-width feature-products-section" id="">
    <div class="pure-u-1">
      <div class="section-label">
        WELCOME TO ANCIENTTREE
      </div>
    </div>
    <div class="pure-u-1 welcome-content-wrapper">
      <div class="pure-g">
        <div class="pure-u-md-1-4 pure-u-lg-1-4"></div>
        <div class="pure-u-1-2 pure-u-md-1-4 pure-u-lg-1-4">
          <div class="welcome-content-left pure-g">
            <div class="pure-u-1">
              “Standing as the earth’s largest and oldest living monuments, I believe these symbolic trees will take on
              a
              greater significance, especially at a time when our focus is directed at finding better ways to live with
              the environment”
            </div>
            <div class="pure-u-1">
              <img src="static/images/tree-logo.jpg">
            </div>
          </div>
        </div>
        <div class="pure-u-1-2 pure-u-md-1-4 pure-u-lg-1-4">
          <div class="welcome-content-right pure-g">
            <div class="pure-u-1">
              “Standing as the earth’s largest and oldest living monuments, I believe these symbolic trees will take on
              a
              greater significance, especially at a time when our focus is directed at finding better ways to live with
              the
              environment”
            </div>
            <div class="pure-u-1 message-icon-wrapper">
              <img src="static/images/message.png">
            </div>
            <div class="pure-u-1 phone-number">
              +86 21 88888888
            </div>
          </div>
        </div>
        <div class="pure-u-md-1-4 pure-u-lg-1-4"></div>
      </div>
    </div>
  </div>
</template>

<style>
.welcome-content-wrapper{
  margin-top: 50px;
}

.welcome-content-left{
  padding-right: 50px;
  font-size: 2rem;
}

.welcome-content-right{
  padding-left: 50px;
  font-size: 2rem;
}

.phone-number {
  color: #8e8888;
  font-size: 2.5rem;
}

.message-icon-wrapper{
  margin-top: 80px;
}
</style>

<script>
    export default{
        name: "WelcomeSection",
        data(){
            return{
            }
        },
        components:{
        }
    }








</script>
