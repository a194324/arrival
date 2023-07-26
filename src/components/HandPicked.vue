<template>
  <div class="handpicked">
<div class="row mb-4">
  <div class="col-md-12 text-center">
    <h2>HandPicked</h2>
  </div>
</div>
    <div class="row">
      <div class="col-md-4 col-sm-12" v-for="property in propeuData" :key="property.id">
        <div class="properties__col">
          <img :src="require(`../assets/images/shopia/kgd/${property.image}.png`)" class="handpicked__img img-fluid" />
        </div>
      </div>
    </div>
</div>
</template>
<script>
export default {
  props: {
    propeuData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>

<style lang="scss">
h3{
font-family: 'Playfair Bold';
font-size: 29.6px;

font-style: italic;
color: #000000;

}





</style>