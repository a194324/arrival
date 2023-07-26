<template>
  <div class="row ">
    <div class="col-md-6 col-sm-12 mkl" v-for="property in propeqData" :key="property.id">
      <div class="properties__col df d-flex ">
        <div class="sf">
        <img :src="require(`../assets/images/shopia/customer/${property.image}.png`)" :alt="property.title"
          class="properties__img img-fluid" />
          </div>
          <div class="tfg">
        <img :src="require(`../assets/images/shopia/customer/fon/${property.image2}.png`)" :alt="property.title"
          class="properties__img img-fluid" />
        <a href="#"><h4 class="properties__h4">{{ property.title }}</h4></a>
        <p class="properties__sub">{{ property.subtitle }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    propeqData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>
<style lang="scss">
.mkl{
max-width: 800px;
background-color:#d9bf8f;
background-repeat: no-repeat;
.sf{
  background-color: transparent;
}
}
.tfg{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.df{
  max-width: 600px;
}
.properties__h4{
  font-family: 'Playfair Bold';
font-size: 30px;
line-height: 17px;
font-weight: 400;
font-style: italic;
color: #000000;

}
.properties__subtitle{
  font-family: Lato;
font-size: 14px;
line-height: 29px;
font-weight: 700;
color: #7f7e7e;
}
</style>
