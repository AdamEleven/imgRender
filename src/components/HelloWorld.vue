<template>
  <div class="percent">
    <!-- <img v-for="(item, index) in imgList" :src="item" alt=""> -->
    {{percent}}
  </div>
</template>

<script>
import {ajax} from '../utils.js';
export default {
  props: ['imgList'],
  data() {
    return {
      count: 0
    }
  },
  computed: {
    percent() {
      let len = this.imgList.length
      return parseInt((this.count / len)*100) + '%'
    }
  },
  mounted() {
    // this.loadImgs();
    this.loadImgBlob();
  },
  methods: {
    loadImgs() {
      let len = this.imgList.length;
      for (let i=0; i<len; i++) {
        let img = new Image();
        img.src = this.imgList[i]
        img.onload = () => {
          this.count++
        }
      }
    },
    loadImgBlob() {
      const that = this;
      for (let i=0; i<that.imgList.length; i++) {
        ajax({ 
          url: that.imgList[i],  // 请求地址
          type: 'GET',  // 请求类型，默认"GET"，还可以是"POST"
          success: function(){  // 请求成功的回调函数
            that.count++
          },
          error: function() {}  // 请求失败的回调函数
        });
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.percent {
  font-size: 50px;
  text-align: center;
}
</style>
