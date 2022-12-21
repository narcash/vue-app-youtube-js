<template>
  <div class="product-list">
    <h1>Письменные столы</h1>
    <ul class="list-default flex">
      <li
        v-for="(product, index) in products"
        :key="index"
      >
        <product-card
          :title="product.title"
          :price="product.price"
          :img-url="product.imgUrl"
          :count="product.count"
        />
      </li>
    </ul>


  </div>
</template>

<script>
import ProductCard from './ProductCard.vue'
  export default {
  name: 'ProductList',
  components: { ProductCard },
  data() {
    return {
      products: [
        {
          title: 'Стол Jim',
          price: 2000 + " $",
          imgUrl: 'https://zeta.kz/upload/ilab/resize_cache/iblock/20d/p1tcbqi0dl9jjfa3bbttlcvh1dhoa2sy.jpg',
          count: 10
        },
        {
          title: 'Стол Monaco',
          price: 3000 + " $",
          imgUrl: 'https://zeta.kz/upload/ilab/resize_cache/iblock/bbd/yji7lpmt1qndlaz1e1v8gytaj9kjn80s.jpg',
          count: 15
        },
        {
          title: 'Стол Jimmy с тумбой',
          price: 5000 + " $",
          imgUrl: 'https://zeta.kz/upload/ilab/resize_cache/iblock/5b4/fpnz3t0im57zftqvqnt56d5qxssz0yw9.jpg',
          count: 19
        }

      ]
    }
  }


  }
</script>

<style lang="sass" scoped>

</style>