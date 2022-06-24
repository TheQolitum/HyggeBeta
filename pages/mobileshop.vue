<template>
<div>
  <div class="mshop">
    <div class="line"></div>
    <div class="m_item"></div>
    <template v-for="(product, $i) in products">
      <productCard
        :product="product"
        :key="$i"
        @popup="popup"
      />
    </template>
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
    ],
    phone: '',
    showSuccess: false,
    showForm: false
  }
},
methods: {
  popup() {
    this.showPopup = true;
    this.showForm = true;
  },
  next() {
    this.showForm = false;
    this.showSuccess = true
  },
  close() {
    this.showPopup = false;
    this.showForm = false;
    this.showSuccess = false;
  }
}
}
</script>

<style lang="css">
*{
  padding: 0;
  margin: 0;
  border: 0;
}
.mshop{
  background-color: wheat;
  width: 100%;
  max-width: 420px;
  height: 550px;
  position: relative;
}
.line{
  margin: 3% auto;
  width: 90%;
  border-bottom: 1px solid black;
}
.m_item{
  width: 315px;
  height: 199px;
  margin: 30px auto;

  background: #FFFFFF;
  box-shadow: 0px 5px 25px 6px rgba(61, 36, 0, 0.42);
  border-radius: 7px;
}
</style>
