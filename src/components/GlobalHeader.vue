<template>
    <div id="global-header" class="pure-g">
      <div class="pure-u-1-3">
        <div id="logo">
          AncientTree
        </div>
      </div>
      <div class="pure-u-1-3"></div>
      <div class="pure-u-1-3">
        <div class="header-menu">HOME</div>
        <div class="header-menu">PRODUCTS</div>
        <div class="header-menu">NEWS</div>
        <div class="header-menu">WHERE TO BUY</div>
      </div>
    </div>
</template>

<style>
#global-header {
    height: 40px;
    width: 100%;
    position: fixed;
    background: #41b883;
    top: 0px;
}

#logo{
    text-align: left;
    padding: 10px;
    font-family: 'Lobster', cursive;
    font-size: 1.2rem;
    color: white;
}

.header-menu {
  display: inline-block;
  padding: 10px;
  color: white;
}
</style>

<script>
export default{
  name: 'GlobalHeader',
  data(){
      return{
          msg:'hello vue'
       }
  }
}
</script>
