<template>
    <div>这是商品列表页面<br />
      <router-link to="/goods/title">显示商品标题</router-link>
      <router-link to="/goods/img">显示商品图片</router-link>
      <div>
        <router-view></router-view>
      </div>
      <router-link v-bind:to="{name: 'Cart'}">跳转到购物车页面</router-link>
    </div>
</template>

<script>
    export default {
        name: "GoodsList",
      methods:{

      }
    }
</script>

<style scoped>

</style>
