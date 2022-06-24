<template>
  <div>
    <div class="m_block1">
    <m_bar />
      <div class="intro_m">
        <p>Островок датского счастья в сердце Сибири!</p>
      </div>
    </div>
    <div class="m_block2">
    <div class="m_fon">
      <p>HYGGE - уютный apres-ski бар, который расположился в самом
        центре горнолыжного курорта Шерегеш, у подножья горы Зелёная.
        Наша команда создаёт настоящий уют и комфорт для гостей.</p>
    </div>
    </div>
    <div class="m_block3">
      <div class="switch">
    <div class="photo_m_switch"></div>
    </div>
    </div>
    <div class="m_block4">
      <div class="m_fon2">
        <p>HYGGE объединяет лучшие блюда датской и европейской кухни.
          В меню предствлены классические датские сморреброды, а так же
          авторские блюда от нашего шефа. Для нашего бара привозим
          необычные сорта крафтового пива и сидра.
        </p>
      </div>
    </div>
    <div class="footer">
    </div>
  </div>
</template>

<script>
import m_bar from "../components/Mobile_ver/m_bar";

export default {
  components: {
    m_bar
  }
}
</script>

<style lang="css">
*{
  padding: 0;
  margin: 0;
  border: 0;
}
.m_block1{
  /*background-color: #B0CB1F;*/
  background-image: url("static/intro mini.jpg");
  width: 100%;
  max-width: 420px;
  height: 550px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  position: relative;
}
.intro_m {
  position: absolute;
  font-size: 34px;
  line-height: 1.2;
  margin: 200px 0 0 22px;
  max-width: 350px;
}
p{
  color: white;
}
.m_block2{
  background-image: url("static/2.png");
  width: 100%;
  max-width: 420px;
  height: 550px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  position: relative;
}
.m_fon{
  position: relative;
  max-height: 175px;
  border-radius: 24px;
  background-color: rgba(0, 0, 0, 0.75);
  font-size: 16px;
  line-height: 1.2;
  margin: 0 auto;
  max-width: 350px;
  top: -30px;
  padding: 14px;
}
.m_block3{
  background-color: white;
  width: 100%;
  max-width: 420px;
  height: 550px;
  position: relative;
}
.photo_m_switch{
  position: relative;
  width: 290px;
  height: 380px;
  top: 50px;
  margin: 0 auto;
  box-shadow: 0px 5px 25px 6px rgba(61, 36, 0, 0.42);
  border-radius: 7px;
}
.m_block4{
  background-image: url("static/photo2.png");
  width: 100%;
  max-width: 420px;
  height: 550px;
  background-repeat: no-repeat;
  /*background-size: cover;*/
  background-position: center;
  position: relative;
}
.m_fon2{
  position: relative;
  max-height: 175px;
  border-radius: 24px;
  background-color: rgba(0, 0, 0, 0.75);
  font-size: 16px;
  line-height: 1.2;
  margin: 0 auto;
  max-width: 350px;
  top: 40px;
  padding: 14px;
}
.footer{
  background-color: #343434;
  height: 10vh;
}
</style>
