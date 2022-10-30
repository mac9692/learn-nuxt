<template>
  <div>
    <h1>상세 페이지</h1>
    <div>
      {{ product }}
      <img :src="product.imageUrl" :alt="product.name" />
      <p>name : {{ product.name }}</p>
      <p>price : {{ product.price }}</p>
      <button @click=""></button>
    </div>

  </div>
</template>

<script>
import {fetchProductById} from "~/api";

export default {
  async asyncData({ params }) {
    const response = await fetchProductById(params.id);
    const product = response.data;
    return { product }
  },
  created() {
    console.log(this.$route.params.id);
  }
}
</script>

<style scoped>

</style>
