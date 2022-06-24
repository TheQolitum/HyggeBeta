<template>
  <div>
  <div class="block1">
    <Navbar />
    <intro />
  </div>
  <div class="block2">
    <second />
  </div>
  <div class="block3">
    <photo />
  </div>
    <div class="block4">
      <third />
    </div>
    <div class="footer">
      <a href="mobile">Мобильная версия сайта</a>
    </div>
    </div>
</template>
<script>

import Navbar from '@/components/Navbar'
import intro from '@/components/text/intro'
import second from '@/components/text/second'
import third from '@/components/text/third'
import photo from '@/components/photo'

export default {
  components: {
    Navbar,
    intro,
    second,
    third,
    photo
  }
}

</script>

<style lang="css">
*{
  padding: 0;
  margin: 0;
  border: 0;
}
.block1 {
  background-image: url("static/intro mini.jpg");
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.block2{
  background-image: url("static/2.png");
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.block3{
  background-color: white;
  height: 100vh;
}
.block4{
  position: relative;
  background-image: url("static/3.png");
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.footer{
  background-color: #343434;
  height: 10vh;
  position: relative;
}
a{
  position: absolute;
  color: white;
  right: 0;
  bottom: 0;
}
</style>
