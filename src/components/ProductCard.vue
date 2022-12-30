<template>
  <div class="product-card">
    <img
      :src="imgUrl"
      width="300px"
    >
    <div class="product-card__info">
      <h2>{{ title }}</h2>
      <p class="price">{{ price }}</p>
      <p class="count">Доступно для доставки: {{ count }} шт</p>
      <button type="button">Добавить в корзину</button>
    </div>
  </div>
</template>

<script>

export default {
  name: 'ProductCard',
  props: ['title', 'price', 'imgUrl']

}
</script>

<style lang="scss">

</style>