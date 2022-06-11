<template>
  <header class="header">
    <div class="header_inner">
      <div class="block_columns_nav">
        <a class="nav_link_shop" href="/"><img src="@/static/logo black.svg" alt=""></a>
      </div>
      <div class="block_columns_nav">
        <a class="nav_link_shop" href="/">Главная</a>
      </div>
      <div class="block_columns_nav">
        <a class="nav_link_shop" href="/shop">Магазин</a>
      </div>
      <div class="block_columns_nav">
        <a class="nav_link_shop" href="https://2gis.ru/sheregesh/firm/70000001041135887/87.888239%2C52.930251?m=87.888272%2C52.930256%2F19.62">Сектор YEAH</a>
      </div>
    </div>
  </header>
</template>

<style lang="css">
.header {
  max-width: 90%;
  margin: 0px auto;
  font-size: 25px;
  padding-top: 3%;
}
img{
  width: 100%;
}
.header_inner {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.block_columns_nav {
  width: 15%;
  text-align: center;
}
.nav_link_shop {
  display: inline-block;
  position: relative;

  text-decoration: none;
  color: black;
  transition: color .2s linear;
}
.nav_link_shop:after {
  content:"";
  display: block;
  width: 100%;
  height: 3px;

  background-color: #B0CB1F;
  opacity: 0;

  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1;

  transition: opacity .2s linear;
}
.nav_link_shop:hover {
  color: #B0CB1F;
}
.nav_link_shop:hover:after {
  opacity: 1;
}
</style>
