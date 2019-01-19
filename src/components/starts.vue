<template>
  <div id="vue_det">
    <h1>site :{{site}}</h1>
    <h1>url : {{url}}</h1>
    <h1>{{details()}}</h1>
  </div>
</template>

<script type="text/javascript">
  var vm = new Vue({
    el: '#vue_det',
    data: {
      site: "初学vue",
      url: "www.baidu.com",
      alexa: "10000"
    },
    method: {
      details: function () {
        return this.site + "-学得不是技术，更是梦想";
      }
    }
  })
</script>

<style scoped>

</style>
