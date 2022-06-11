<template>
  <div>
    <div class="shop">
      <template v-for="(product, $i) in products">
        <productCard
          :product="product"
          :key="$i"
          @popup="popup"
        />
      </template>
      <div id="popup" class="popup" v-if="showPopup" style="z-index: 9999">
        <a href="" class="popup_area"></a>
        <div class="popup_body">
          <div class="popup_content">
            <a href="" class="popup_close">X</a>
            <div class="popup_title">Спасибо, что выбрали нас!</div>
            <div class="popup_text">Для оформления заказа,
              оставьте свое имя и номер телефона. В течении 2-х часов с вами
              свяжется наш менеджер.</div>
            <input type="name" size="20" placeholder="Ваше имя">
            <input type="number" pattern="[0-9]" placeholder="+7-(9**)-***-**-**">
            <button>Отправить</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>


export default {

  data() {
    return {
      showPopup: false,
      products : [
        {
          class: 'pol1',
          price: 125,
          name: 'Мед',
          weight: 250,
          typeString: 'Вид меда: цветочный',
        },
        {
          class: 'pol2',
          price: 240,
          name: 'Мед',
          weight: 500,
          typeString: 'Вид меда: цветочный',
        },

        {class: 'pol3',
          price: 470,
          name: 'Мед',
          weight: 1000,
          typeString: 'Вид меда: цветочный',
        },
        {
          class: 'pol4',
          price: 100,
          name: 'Орехи',
          weight: 100,
          typeString: 'Вид орехов: фундук',
        },
        {
          class: 'pol5',
          price: 260,
          name: 'Орехи',
          weight: 300,
          typeString: 'Вид орехов: фундук',
        },
        {
          class: 'pol6',
          price: 900,
          name: 'Орехи',
          weight: 1000,
          typeString: 'Вид орехов: фундук',
        },
        {
          class: 'pol7',
          price: 300,
          name: 'Сироп',
          weight: 250,
          typeString: 'Вид сиропа: клен',
        },
        {
          class: 'pol8',
          price: 550,
          name: 'Сироп',
          weight: 500,
          typeString: 'Вид сиропа: клен',
        },
        {
          class: 'pol9',
          price: 1000,
          name: 'Сироп',
          weight: 1000,
          typeString: 'Вид сиропа: клен',
        },
      ]
    }
  },
  methods: {
    popup() {
      console.log('asdfasdf');
      this.showPopup = true;
    }
  }
}
</script>

<style lang="css">
.shop{
  height: 45vh;
  /*height: 45%;*/
  width: 90%;
  margin: 0 auto;

  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.shop p{
  color: black;
  text-decoration: none;
}
a{
  text-decoration: none;
  color: black;
}

.block_columns_shop{
  position: relative;
  width: 29%;
  height: 60%;
  margin: 0 0 5% 0;
}
.block_item {
  position: relative;
  width: 100%;
  height: 100%;

  background-color: white;
  box-shadow: 0px 5px 25px 6px rgba(61, 36, 0, 0.42);
  border-radius: 7px;
  display: flex;
  flex-flow: row nowrap;
}
.pol1{
  background-image: url("static/honey.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.description{
  margin: 4%;
  width: 50%;
  position: relative;
}
.pol2{
  background-image: url("static/honey.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.pol3{
  background-image: url("static/honey.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.pol4{
  background-image: url("static/nuts.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.pol5{
    background-image: url("static/nuts.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.pol6{
    background-image: url("static/nuts.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.pol7{
    background-image: url("static/syrup.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.pol8{
    background-image: url("static/syrup.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.pol9{
    background-image: url("static/syrup.png");
  margin: 0 0 0 3%;
  background-repeat     : no-repeat;
  background-size       : cover;
  background-position-x : 50%;
  background-position-y : 50%;
  width: 100%;
  height: 100%;
  max-width: 212px;
  max-height: 212px;
}
.popup{
  position: fixed;
  width: 100%;
  height: 100%;
  background-color: rgba(50, 50, 50, 0.44);
  top: 0;
  left: 0;
  opacity: 0;
  visibility: hidden;
  transition: all 0.8s ease 0s;
}
.popup:target{
  opacity: 1;
  visibility: visible;
}
.popup_area{
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
}
.popup_body{
  min-height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.popup_content{
  max-width: 600px;
  background-color: #B0CB1F;
  border-radius: 30px;
  padding: 40px;
  position: relative;
}
.popup_close{
  position: absolute;
  right: 10px;
  top: 10px;
  text-decoration: none;
  color: black;
  font-size: 20px;
}
.popup_title{
  font-size: 24px;
  margin: 10px 0 30px 40px;
}
.popup_text{
  padding: 30px;
}
input{
  margin: 10px auto;
  display: block;
  width: 50%;
  padding: 0.375rem 0.75rem;
  font-family: inherit;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5;
  color: #212529;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #bdbdbd;
  border-radius: 0.25rem;
  transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
}
button{
  background-color: black;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  border-radius: 20px;
  margin: 20px 0 0 50%;
}
</style>
