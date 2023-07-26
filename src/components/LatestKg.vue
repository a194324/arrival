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
      <div class="col-md-3 col-sm-12" v-for="property in prData" :key="property.id">
        <div class="properties__col">
          <img :src="require(`../assets/images/arrivel/pr/${property.image}.jpg`)"
            class="properties__img img-fluid fop" />
          <h4 class="properties__h4">{{ property.title }}</h4>
          <p class="properties__price">{{ property.price }}</p>
        </div>
      </div>
    </div>
    </div>
  </template>
  <script>
  export default {
    props: {
      prData: {
        type: Array,
        default: () => [],
      },
    },
  }
  </script>

  <style lang="scss">

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
