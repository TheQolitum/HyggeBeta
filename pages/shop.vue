<template>
  <div>
    <div class="block1">
      <shop_bar />
      <div class="line"></div>
      <shop_item />
    </div>
    <div class="shop_footer">
      <a href="mobileshop.vue">Мобильная версия сайта</a>
    </div>
  </div>
</template>

<script>

import shop_bar from '@/components/shop_bar'
import shop_item from '@/components/shop_item'
import popup from '@/components/popup'

export default {
  components: {
    shop_bar,
    shop_item,
    popup
  }
}

</script>

<style lang="css">
*{
  padding: 0;
  margin: 0;
  border: 0;
}
.block1{
  position: relative;
  background-color: white;
  height: 125vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.line {
  margin: 3% auto;
  width: 90%;
  border-bottom: 1px solid black;
}
.shop_footer{
  position: relative;
  background-color: #343434;
  height: 10vh;
}
a{
  position: absolute;
  color: white;
  right: 0;
  bottom: 0;
}
</style>
