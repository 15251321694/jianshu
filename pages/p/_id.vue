<template>
  <div>
      <my-header></my-header>
       <div class="note">
            <div class="post">
                   <div class="article">
                       <h1 class="title">对简书作者要说的四点免费建议</h1>
                       <div class="author">
                            <div class="avatar">
                                <img src="~/assets/img/default-avatar.jpg">
                            </div>
                            <div class="info">
                                 <nuxt-link class="name" to="name">
                                  世代
                                 </nuxt-link>
                                <a href="javascript:void(0)" class="btn btn-follow">
                                    <i class="fa fa-plus"></i>
                                <span>关注</span>
                                </a>
                              <div class="meta">
                                <span class="publish-time">
                                    2018.04.12 17:51*
                                </span>
                                <span class="wordage">
                                    字数 1038
                                </span>
                                <span class="view-count">
                                    阅读 20138
                                </span>
                                <span class="comment-count">
                                    评论 181
                                </span>
                                <span class="like-count">
                                    喜欢 673
                                </span>
                                <span class="rewards-count">
                                    赞赏 29
                                </span>
                              </div>
                          </div>

                        </div>
                            <div class="show-content">
                                <p>简书版权是为作者服务的。到现在为止我们做得还不错，接近80部作品签约出版了，从4月份开始，陆续会有一些纸书会面世。更让人开心的是，我们的非虚构类作者，有的已经拿到了起印三万册的条件，而虚构类作者，有的拿到了起印一万册的条件。</p>
                                <p>对于国内的新人作者来说，这绝对是最高的条件。我和我的同事要谢谢你们，是你们的才华和努力让简书版权成为目前国内最好的新人发现和孵化机构。</p>
                            </div>
                       </div>
                            <div class="show-foot">
                                <nuxt-link class="notebook" to="/note/123">
                                     <i class="fa fa-book"></i>
                                    日记本
                                </nuxt-link>
                                <div class="copyright">
                                    © 著作权归作者所有 
                                </div>
                            </div>
                        <!-- 文章底部的作者信息 -->
                <div class="follow-detail">
                  <div class="info">
                      <div class="avatar">
                          <img src="~/assets/img/default-avatar.jpg" alt="">
                      </div>
                      <a href="javascript:void(0)" class="btn-follow">
                          <i class="fa fa-plus"></i>
                          <span>关注</span>
                      </a>
                      <nuxt-link to="/u/123" class="title">
                        世代
                      </nuxt-link>
                      <i class="fa fa-mars"></i>
                      <p>写了 74603 字，被 2059 人关注，获得了 1971 个喜欢</p>
                   </div>
                 </div>
                 <div class="meta-bottom">
                    <div class="like" :class="{'islike':islike}" @click="islike=!islike">
                        <div class="like-btn">
                            <a href="javascript:void(0)">喜欢</a>
                        </div>
                        <div class="like-num">
                            <a href="javascript:void(0)">673</a>
                        </div>
                    </div>
                    
                    <div class="share">
                        <a href="javascript:void(0)" class="share-btn" v-tooltip="'分享到微信'">
                            <i class="fa fa-weixin weixin"></i>
                        </a>
                        <a href="javascript:void(0)" class="share-btn" v-tooltip="'分享到微博'">
                            <i class="fa fa-weibo weibo"></i>
                        </a>
                        <a href="javascript:void(0)" class="share-btn" v-tooltip="'分享到qq'">
                            <i class="fa fa-qq qq"></i>
                        </a>
                        <v-popover class="more-share share-btn">
                          <a href="javascript:void(0)" class="more-share tooltip-target">
                          更多分享
                      </a>
                      <template slot="popover">
                          <div >
                            <ul class="popover">
                                <li>
                                    <i class="fa fa-star"></i>
                                    分享到QQ空间
                                </li>
                                <li>
                                    <i class="fa fa-twitter"></i>
                                    分享到Twitter
                                </li>
                                <li>
                                    <i class="fa fa-facebook-official"></i>
                                    分享到Facebook
                                </li>
                                <li>
                                    <i class="fa fa-google-plus"></i>
                                    分享到Google+
                                </li>
                                <li>
                                    <i class="dou">豆</i>
                                    分享到豆瓣
                                </li>    
                            </ul>
                            </div>
                      </template>
                      </v-popover>
                    </div>
                 </div>
                 <!-- 留言组件 -->
                 <my-comment></my-comment>
                    </div>
                </div>
             </div>
</template>
<script>
import myComment from "~/components/myComment";
import myHeader from "~/components/myHeader";
import Vue from 'vue'
import VTooltip from 'v-tooltip'
Vue.use(VTooltip)
export default {
  data() {
    return {
      name: "page",
      islike: false,
      isWeixin:false,
      isWeibo:false,
      isqq:false
    };
  },
  components: {
    myHeader,
    myComment
  }
};
</script>

