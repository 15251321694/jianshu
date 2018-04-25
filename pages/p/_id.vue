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
                                <a href="#" class="btn btn-follow">
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
                      <a href="#" class="btn-follow">
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
                    <div class="like">
                        <div class="like-btn">
                            <a href="#" class="">喜欢</a>
                        </div>
                        <div class="like-num">
                            <a href="#">673</a>
                        </div>
                    </div>
                    <div class="share">
                        <a href="#" class="share-btn">
                            <i class="fa fa-weixin weixin"></i>
                        </a>
                        <a href="#" class="share-btn">
                            <i class="fa fa-weibo weibo"></i>
                        </a>
                        <a href="#" class="share-btn">
                            <i class="fa fa-qq qq"></i>
                        </a>
                        <a href="#" class="share-btn more-share">
                            更多分享
                        </a>
                    </div>
                 </div>
                 <!-- 留言组件 -->
                 <my-comment></my-comment>
                    </div>
                </div>
             </div>
</template>
<script>
import myHeader from "~/components/myHeader";
import myComment from "~/components/myComment";
export default {
  head: {
    title: "简书文章详情页面-创作你的创作",
    meta: [
      { charset: "utf-8" },
      { name: "keywords", content: "文章详情页面" },
      { name: "description", content: "文章页面" }
    ]
  },
  data() {
    return {};
  },
  components: {
    myHeader,
    myComment
  }
};
</script>