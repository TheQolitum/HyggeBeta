<template>
  <div>
    <div class="block1">
      <shop_bar />
      <div class="line"></div>
      <shop_item />
    </div>
    <popup />
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
  height: 200vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.line {
  margin: 3% auto;
  width: 90%;
  border-bottom: 1px solid black;
}
</style>
