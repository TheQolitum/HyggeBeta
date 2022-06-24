<template>
  <div>
    <div class="ms_bar">
      <div class="content">
        <div class="logo_column">
          <a class="nav_link" href="/"><img src="static/logo_black.svg" alt=""></a>
        </div>
        <div class="menu_column">
          <a class="nav_link " href="/"><img src="static/menu.png" alt=""></a>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="css">
.ms_bar {
  position: absolute;
  max-width: 90%;
  width: 420px;
  margin: 22px;
  font-size: 16px;
  /*padding-top: 3%;*/
}
.content{
  display: flex;
  position: relative;
  justify-content: space-between;
  align-items: center;
}
.logo_column{
  max-width: 200px;
  width: 75%;
  max-height: 55px;
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.menu_column{
  background-image: url("static/menu.png");
  max-width: 31px;
  max-height: 58px;
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
</style>
