<template>
  <div>
        <div class="row text-center">
          <div class="col-md-12">
            <h2 class="properties__h2">
             <b>FEATURED</b> ARRIVALS
            </h2>
          </div>
          <div class="col-md-12">
            <p class="properties__subtitle">
             “Whoever said money cant buy happiness simply didn t know WHERE TO SHOP”
            </p>
          </div>
        </div>
  <div class="row">
    <div class="col-md-3 col-sm-12" v-for="property in prolData" :key="property.id">
      <div class="properties__col">
        <img :src="require(`../assets/images/arrivel/prol/${property.image}.jpg`)"
          class="properties__img img-fluid fop" />
        <h4 class="properties__h4">{{ property.title }}</h4>
        <p class="properties__price">{{ property.price }}</p>
        <button type="button" class="btn btn-warning nj">Warning</button>
      </div>
    </div>
  </div>
  </div>
</template>
<script>
export default {
  props: {
    prolData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>

<style lang="scss">
.nj{
 margin: 0 auto;
display: block;
position: relative;
top: -16px;
}
.fop{
  object-fit: cover;
        width: 100%;
        height: 100%;
        transition: 1s;
        &:hover{
          transform:scale(1.2);
        }
}
</style>