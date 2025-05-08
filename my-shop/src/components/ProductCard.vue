<template>
  <div class="product-card">
    <img class="product-image" src="image" :alt="name" />
    <h2>{{ name }}</h2>
    <p>{{ description }}</p>
    <p class="price">{{ price }} грн</p>
    <button class="buy-button">Купити</button>
  </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props: {
    image: String,
    name: String,
    description: String,
    price: Number
  }
}
</script>

<style scoped>
.product-card {
  max-width: 300px;
  border: 1px solid #e0e0e0;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
  padding: 16px;
}

.product-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.price {
  font-size: 18px;
  font-weight: bold;
  color:rgb(217, 208, 31);
}

.buy-button {
  background-color:rgb(0, 0, 0);
  color: #fff;
  font-weight: bold;
  border: none;
  border-radius: 6px;
  padding: 10px 20px;
  cursor: pointer;
  margin-bottom: 20px;
}

.buy-button:hover {
  background-color:rgb(231, 216, 49);
}
</style> 