<template>
  <div class="percent">
    <!-- <img v-for="(item, index) in imgList" :src="item" alt=""> -->
    {{percent}}
  </div>
</template>

<script>
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
    this.loadImgs();
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
