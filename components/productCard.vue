<template>
  <div class="block_columns_shop">
    <div class="block_item">
      <div :class="product.class">
      </div>
      <div class="description">
        <p>Продукт: {{product.name}}</p>
        <p>Вес товара, г: {{ product.weight}}</p>
        <p>{{ product.typeString }}</p>
        <p>Страна изготовитель: Россия</p>
        <p>Цена руб.: {{ product.price }}</p>
        <div class="buy" @click="$emit('popup')">Купить</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      product: {
        class: 'pol',
        price: 0,
        name: '',
        weight: 0,
        typeString: '',
      }
    }
  },
  props: ['product'],
  name: "productCard"
}
</script>

<style scoped>
.buy{
  font-size: 30px;
  position: absolute;
  margin: 15px 0 0 70px;
  border: black solid 1px;
  border-radius: 5px;
}
</style>
