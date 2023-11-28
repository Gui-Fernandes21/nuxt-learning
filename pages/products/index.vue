<template>
  <h1>Enter the ID of your product</h1>
  <input type="text" v-model="prodId">
  <button @click="loadProduct">Search Product</button>

  <br>
  <br>

  <nuxt-link to="/products/1">Product 1</nuxt-link>
  <br>
  <nuxt-link to="/products/2">Product 2</nuxt-link>
</template>

<script>
export default {
  data() {
    return {
      prodId: ''
    }
  },
  methods: {
    loadProduct() {
      this.$router.push('/products/' + this.prodId);
    }
  }
}
</script>