<template>
    <div class="row">
    <div class="col-md-12 text-center">
      <h2>Our Brand</h2>
    </div>
    </div>
    <div class="row">
      <div class="col-md-4 col-sm-12" v-for="property in propejData" :key="property.id">
        <div class="properties__col text-center">
          <a href="#"><img :src="require(`../assets/images/shopia/cart/fots/${property.image}.png`)" class="properties__img bh img-fluid" /></a>
        </div>
      </div>
    </div>
</template>
<script>
export default {
  props: {
    propejData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>
<style lang="scss">
.bh{
  max-width: 230px;
}
</style>