<template>
    <div>
        <form class="new-comment" method="post">
            <slot></slot>
            <textarea name="comment-content" placeholder="写下你的评论"></textarea>
            <div class="write-function-block">
                <div class="emoji-modal-wrap">
                    <a href="javascript:void(0)" class="emoji" @click="isEmoji=!isEmoji">
                        <i class="fa fa-smile-o"></i>
                    </a>
                    <div class="emoji-modal" v-show="isEmoji">
                        <my-emoji></my-emoji>
                    </div>
                </div>
                <div class="hint">Ctrl+Enter发送</div>
                <a href="#" class="btn-send">发送</a>
                <a href="#" class="btn-cancel">取消</a>
            </div>
        </form>
    </div>
</template>
<script>
import myEmoji from '~/components/myEmoji'
export default {
  name: "myForm",
  data() {
    return {
        isEmoji:false
    };
  },
  components:{
      myEmoji
  }
};
</script>