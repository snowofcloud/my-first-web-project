<template>
    <!--文本插值法-->
    <!--<div id="app">
      <p>{{message}}</p>
    </div>-->
  <!--Html插值法-->
  <!--<div id="app">
    <div v-html="message"></div>
  </div>-->
  <!--属性插值法-->
  <div class="starts2">
    <label for="r1">修改颜色</label><input type="checkbox" v-model="use" id="r1"/>
    <br/>
    <div v-bind:class="{'class':use}">
      v-bind:class 指令
    </div>
  </div>

</template>

<script>
   //文本插值法
    /*new Vue({
      el: '#app',
      data: {
        message: 'hello vue.js!!!'
      }
    })*/
    //Html插值法
  /*new Vue({
    el: '#app',
    data: {
      message: '<h1>Html插值法</h1>'
    }
  })*/
  //属性插值法
  new Vue({
    el: 'starts2',
    data:{
      use:false
    }
  });
</script>

<style>

</style>
