<style scoped lang="scss">
  ul{
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    border-top: 1px solid #999;
    padding: 5px 20px;
  }
  li {
    .img {
      text-align: center;
      img {
        width: 28px;
        height: 28px;
      }
    }
  }
  li.active {
    color: #00b28c;

  }
</style>
<template>
  <ul>
    <router-link :to="{name: 'Home'}" tag="li">
      <div class="img"><img src="../../assets/svg/home.svg" alt=""></div>
      <div>首页</div>
    </router-link>
    <router-link :to="{name: 'Categories'}" tag="li">
      <div class="img"><img src="../../assets/svg/category.svg" alt=""></div>
      <div>分类</div>
    </router-link>
    <router-link :to="{name: 'Cart'}" tag="li">
      <div class="img"><img src="../../assets/svg/cart.svg" alt=""></div>
      <div>购物车</div>
    </router-link>
    <router-link :to="{name: 'Me'}" tag="li">
      <div class="img"><img src="../../assets/svg/me.svg" alt=""></div>
      <div>我的</div>
    </router-link>
  </ul>
</template>
<script>
    export default {
        data() {
            return {
                msg: 'hello world'
            }
        },
        components: {}
    }
</script>
