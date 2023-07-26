<template>
  <div class="row">
<div class="col-md-12 text-center mb-5">
    <h4 class="zxcv">Summer Collection</h4>
    </div>
  </div>
  <div class="row">
    <div class="col-md-3 col-sm-12" v-for="property in propelData" :key="property.id">
      <div class="properties__col">
        <img :src="require(`../assets/images/shopia/cart/kg/${property.image}.png`)" :alt="property.title"
          class="properties__img img-fluid" />
        <a href="#"><h4 class="properties__h4">{{ property.title }}</h4></a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    propelData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>
<style lang="scss">
.zxcv{
  font-weight: 700;
}
 a{
  text-decoration: none !important;
}
.img-fluid{
  width: 100%;
  object-fit: cover;
  height: auto;
}
</style>