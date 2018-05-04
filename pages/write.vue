<template>
  <div id="root">
      <div class="ant-row _1gp6t">
           <div class="ant-col-4 _2v5v5">
               <div class="_3zibT">
                   <nuxt-link to="/">
                    回首页
                   </nuxt-link>
               </div>
               <div class="_1iZMb">
                   <div class="_33Zlg">
                       <i class="fa fa-plus"></i>
                       <span>新建文集</span>
                   </div>
               </div>
               <ul>
                   <li>
                       <span>日记本</span>
                       <i class="fa fa-gear"></i>
                   </li>
                   <li>
                       <span>随笔</span>
                   </li>
               </ul>
          </div>
      </div>
  </div>
</template>
<script>
import Vue from "vue";
import VTooltip from "v-tooltip";
Vue.use(VTooltip);
export default {
  data() {
    return {
      name: "写文章"
    };
  },
  components: {}
};
</script>
<style scoped>
#root {
  width: 100%;
  height: 100%;
  max-width: 100vw;
  max-height: 100vh;
}
._1gp6t{
    height: 100%;
    overflow: hidden;
}
.ant-row{
    position: relative;
    margin-left: 0%;
    margin-right: 0%;
    zoom: 1;
    display: block;
    box-sizing: border-box;
}
._2v5v5 {
  position: relative;
  height: 100%;
  overflow: auto;
  background-color: #404040;
  color: #f2f2f2;
  z-index: 100;
}
.ant-col-4 {
  width: 16.7%;
  display: block;
  box-sizing: border-box;
}
</style>
