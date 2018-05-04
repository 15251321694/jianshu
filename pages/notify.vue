<template>
  <div>
      <my-header></my-header>
      <div class="container index">
        <div class="row">
            <div class="aside">
                <ul class="dropdown-menu">
                    <li>
                        <nuxt-link to="/notify">
                        <i class="fa fa-comment-o"></i>
                        <span>评论</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/chats">
                        <i class="fa fa-envelope-o"></i>
                        <span>简信</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/requests">
                        <i class="fa fa-upload"></i>
                        <span>投稿请求</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/likes">
                        <i class="fa fa-heart-o"></i>
                        <span>喜欢和赞</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/fllows">
                        <i class="fa fa-user-plus"></i>
                        <span>关注</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/money">
                        <i class="fa fa-jpy"></i>
                        <span>赞赏和付费</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/others">
                        <i class="fa fa-ellipsis-h"></i>
                        <span>其它提醒</span>
                        </nuxt-link>
                    </li>
                </ul>
            </div>
            <div class="col-xs-16 col-xs-offset-8 main">
                <div class="menu">收到的评论</div>
                <ul class="comment-list"></ul>
                <div class="find-nothing">
                    <img src="~/assets/img/kb.png">
                    <div>这里还木有内容哦~</div>
                </div>
            </div>
        </div>
      </div>
  </div>
</template>
<script>
import myHeader from "~/components/myHeader";
import Vue from "vue";
import VTooltip from "v-tooltip";
Vue.use(VTooltip);
export default {
  data() {
    return {
      name: "消息"
    };
  },
  components: {
    myHeader
  }
};
</script>
<style scoped>
.aside {
  width: 218.75px;
  position: fixed;
  top: 0;
  bottom: 0;
  margin: 86px 0 0;
  padding: 0 0 30px;
  overflow: auto;
}
.main {
  margin-left: 34%;
}
.dropdown-menu{
  background: #fff;
  position: absolute;
  left: 0;
  min-width: 160px;
  z-index: 999;
  margin: 0;
  padding: 10px 0;
  font-size: 15px;
}
.dropdown-menu li a{
  padding: 10px 20px;
  display: block;
  line-height: 30px;
}
.dropdown-menu li a:hover {
  background-color: #f5f5f5;
}
.dropdown-menu li a i {
  margin-right: 10px;
  color: #ea6f5a;
  width: 20px;
  display: inline-block;
  font-size: 20px;
}
.menu{
   margin-bottom: 20px;
   font-size: 14px;
   font-weight: 700;
}
.find-nothing{
    margin-top: 150px;
    text-align: center;
}
.find-nothing img{
    width: 100px;
    vertical-align: middle;
    border: 0;
}
.find-nothing div{
    margin-top: 20px;
    font-size: 14px;
    font-weight: 700;
}
</style>
