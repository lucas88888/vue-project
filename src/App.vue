<!-- App.vue -->

<template>
  <div id="app">
    <Header />
    <ProductList :products="products" />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import ProductList from './components/ProductList.vue';

export default {
  name: 'App',
  components: {
    Header,
    Footer,
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
          image: '1.png'
        },
        {
          id: 2, 
          name: 'Smartwatch 4.0', 
          description: 'Verfolgen Sie Ihre Fitnessziele mit der neuesten Smartwatch-Technologie.', 
          price: '299.99', 
          rating: 4.0,
          image: '2.png'
        },
        {
          id: 3, 
          name: 'Wireless Kopfhörer', 
          description: 'Hochwertiger Sound und Freiheit ohne Kabel.', 
          price: '89.99', 
          rating: 3,
          image: '3.png' // Updated image name
        }
      ]
    };
  }
};
</script>

<style>

body {
  background-color: #000; 
  color: #fff; 
}


</style>