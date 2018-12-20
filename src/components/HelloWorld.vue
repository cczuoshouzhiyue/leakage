<template>
  <div class="hello" v-if="isDestory">
    这是页面1
    <div class="block">
      <span class="demonstration">默认 Hover 指示器触发</span>
      <el-carousel height="150px">
        <el-carousel-item v-for="item in 4" :key="item">
          <h3>{{ item }}</h3>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      isDestory: true
    }
  },
  beforeDestroy () {
    this.isDestory = false
  }
}
</script>
