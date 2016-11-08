<template>
  <div id="global-header" class="pure-g">
    <div class="pure-u-1 pure-u-md-2-5 pure-u-lg-2-5">
      <div class="pure-g">
        <div class="pure-u-1-2">
          <div id="logo">
            AncientTree
          </div>
        </div>
        <div class="pure-u-1-2">
          <div id="menu-toggle-button-wrapper" v-on:click="collapseMenu">
            <Icon name="list" scale="2" id="menu-toggle-button"></Icon>
          </div>
        </div>
      </div>
    </div>
    <div class="pure-u-1 pure-u-md-3-5 pure-u-lg-3-5" v-if="!compactMode || (compactMode && menuCollapsed)">
      <div class="pure-g full-height">
        <div class="header-menu pure-u-1 pure-u-md-1-4 pure-u-lg-1-4">HOME</div>
        <div class="header-menu pure-u-1 pure-u-md-1-4 pure-u-lg-1-4">PRODUCTS</div>
        <div class="header-menu pure-u-1 pure-u-md-1-4 pure-u-lg-1-4">NEWS</div>
        <div class="header-menu pure-u-1 pure-u-md-1-4 pure-u-lg-1-4">WHERE TO BUY</div>
      </div>
    </div>
  </div>
</template>

<style>

@media screen and (max-width: 767px) {
  #global-header {
    height: 50px;
    width: 100%;
    position: fixed;
    background: #41b883;
    top: 0px;
  }
  #menu-toggle-button-wrapper{
    text-align: right;
    display: block!important;
    padding: 10px 10px 0 0;
    cursor: pointer;
  }

  #menu-toggle-button{
    color: white;
  }

}

@media screen and (min-width: 768px) {
  #global-header {
    height: 50px;
    width: 100%;
    position: fixed;
    background: #41b883;
    top: 0px;
  }

  #menu-toggle-button{
    display: none!important;
  }

}

#logo{
    text-align: left;
    padding: 10px 0 10px 10px;
    font-family: 'Lobster', cursive;
    font-size: 1.2rem;
    color: white;
}

.header-menu {
  display: inline-block;
  padding: 15px 0 15px 0;
  color: white;
  cursor: pointer;
  background-color: #41b883;
}

.header-menu:hover{
  background-color: #388E3C;
}

</style>

<script>
import Vue from 'vue'
import Icon from '../vue-awesome/components/Icon.vue'
import '../vue-awesome/icons'
export default{
  name: 'GlobalHeader',
  components: {
    Icon
  },
  data(){
      return{
          msg:'hello vue',
          menuCollapsed: false,
          compactMode: true
       }
  },
  methods:{
    collapseMenu(){
      this.menuCollapsed = !this.menuCollapsed;
    },
    handleGlobalHeaderOnWindowResize(event){
      console.log(document.documentElement.clientWidth);
      console.log(document.documentElement.clientHeight);
      if(this.isCompactMode(document.documentElement.clientWidth)){
        this.menuCollapsed = false;
        this.compactMode = true;
      }else{
        this.compactMode = false;
      }
    },
    isCompactMode(width){
      return width < 768;
    }
  },
  mounted(){
    this.compactMode = this.isCompactMode(document.documentElement.clientWidth)?true:false;
    this.$nextTick(function(){
      window.addEventListener('resize', this.handleGlobalHeaderOnWindowResize);
    })
  }
}

</script>
