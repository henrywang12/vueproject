<template>
  <div id="app">
    <v-header></v-header>
    <div class="tab">
      <div class="tab-item">商品</div>
      <div class="tab-item">评论</div>
      <div class="tab-item">商家</div>
    </div>
    <div class="content">
      .
    </div>
  </div>
</template>

<script>
import header from './components/header/header.vue'
export default {
  name: 'app',
  components: {
    'v-header': header
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
  margin-top: 60px;
}
  #app .tab {
    display: flex;
    width: 100%;
    height: 40px;
    line-height: 40px;
    border: 1px solid red;
  }
    .tab-item{
      flex:1;
    }
  #app .content{
    width:100%;
    height:100%;
    border:1px solid green;
  }
</style>
