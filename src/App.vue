<template>
  <div id="app">
    <ProductList :products="products" />
  </div>
</template>

<script>
import ProductList from './components/ProductList.vue';

export default {
  name: 'App',
  components: {
    ProductList
  },
  data() {
    return {
      products: [
        { 
          id: 1, 
          name: 'Outdoor Zelt', 
          description: 'Robustes Zelt für alle Outdoor-Abenteuer.', 
          price: '149.99', 
          rating: 2,
          image: '3.png'
        },
        {
          id: 2, 
          name: 'Smartwatch 4.0', 
          description: 'Verfolgen Sie Ihre Fitnessziele mit der neuesten Smartwatch-Technologie.', 
          price: '299.99', 
          rating: 4.0,
          image: '1.png'
        },
        {
          id: 3, 
          name: 'Wireless Kopfhörer', 
          description: 'Hochwertiger Sound und Freiheit ohne Kabel.', 
          price: '89.99', 
          rating: 3,
          image: '2.png' // Updated image name
        }
      ]
    };
  }
};
</script>

<style>
/* Globale Stile, falls benötigt */
</style>
