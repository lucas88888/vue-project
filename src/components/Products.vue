<script>
import Product from "./Products.vue";

export default {
  components: {
    Product,
  },
  data() {
    return {
      products: [
        {
          id: "1",
          imageUrl: "https://loremflickr.com/150/150?random=1",
          productName: "Product 1",
          releasedDate: "May 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 4,
        },
        {
          id: "2",
          imageUrl: "https://loremflickr.com/150/150?random=2",
          productName: "Product 2",
          releasedDate: "October 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 2,
        },
        {
          id: "3",
          imageUrl: "https://loremflickr.com/150/150?random=3",
          productName: "Product 3",
          releasedDate: "May 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 5,
        },
      ],
    };
  },
};
</script>
<template>
  <div v-for="product in products" :key="product.id">
    <Product :data="product" />
  </div>
</template>