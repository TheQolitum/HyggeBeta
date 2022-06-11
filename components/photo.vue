<template>
  <div class="photos">

  <div class="block_photo">
  <div class="block_columns">
    <div class="block_item">
      <div class="photo1"></div>
    </div>
  </div>

  <div class="block_columns1">
    <div class="block_item1">
      <div class="photo2"></div>
    </div>
  </div>

  <div class="block_columns">
    <div class="block_item">
      <div class="photo3"></div>
    </div>
  </div>
  </div>

  <div class="block_photo1">
    <div class="block_columns1">
      <div class="block_item1">
        <div class="photo4"></div>
      </div>
    </div>

    <div class="block_columns">
      <div class="block_item">
        <div class="photo5"></div>
      </div>
    </div>

    <div class="block_columns1">
      <div class="block_item1">
        <div class="photo6"></div>
      </div>
    </div>
  </div>

  </div>
</template>

<style lang="css">

.photos {
  height: 100%;
  width: 100%;
}

.block_columns{
  width: 29%;
  height: 60%;
}

.block_columns1{
  width: 29%;
  height: 125%;
}

.block_photo{
  position: relative;
  height: 45%;
  width: 90%;
  top: 5%;
  margin: 0 auto;

  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.block_photo1{
  position: relative;
  height: 45%;
  width: 90%;
  top: 5%;
  margin: 0 auto;

  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}

.block_item{
  position: relative;
  width: 100%;
  height: 100%;
  align-items: center;

  box-shadow: 0px 5px 25px 6px rgba(61, 36, 0, 0.42);
  border-radius: 7px;

}

.block_item1{
  width: 100%;
  height: 100%;


  box-shadow: 0px 5px 25px 6px rgba(61, 36, 0, 0.42);
  border-radius: 7px;
}

.photo1{
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  background-image: url("static/2.png");
  border-radius: 7px;
}
.photo2{
  background-repeat     : no-repeat;
  /*background-size       : cover;*/
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  background-image: url("static/photo2.png");
  border-radius: 7px;
}
.photo3{
  background-repeat     : no-repeat;
  /*background-size       : cover;*/
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  background-image: url("static/photo3.png");
  border-radius: 7px;
}
.photo4{
  background-repeat     : no-repeat;
  /*background-size       : cover;*/
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  background-image: url("static/photo4.png");
  border-radius: 7px;
}
.photo5{
  background-repeat     : no-repeat;
  /*background-size       : cover;*/
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  background-image: url("static/photo5.png");
  border-radius: 7px;
}
.photo6{
  background-repeat     : no-repeat;
  /*background-size       : cover;*/
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  background-image: url("static/photo6.png");
  border-radius: 7px;
}

</style>
