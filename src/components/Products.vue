<template>
    <div>
      <div class="container">
        <div class="row row-cols-1 row-cols-sm-2 row-cols-lg-3">
          <div class="col" v-for="item in product" :key="item.id">
            <div class="card" style="width: 18rem">
              <img :src="item.image" class="card-img-top" :alt="item.title" />
              <div class="card-body">
                <h1>{{ item.title }}</h1>
                <h4>{{ item.price }}</h4>
              </div>
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
      product: [],
    };
  },
  methods: {
    async fetchData() {
      const res = await fetch(
        "https://ganiefah.github.io/productsJSONserver/products.json"
      );
      let parsedProducts = await res.json();
      this.product = parsedProducts.products;
    },
  },
  mounted() {
    this.fetchData();
  },
};
</script>

<style scoped>
.container {
    height: max-content;
}

</style>