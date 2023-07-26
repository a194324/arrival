<template>
  <div class="home">
    <MainContainer>
       <ArrivalsKg/>
      <FeaturedArrivals :prolData="prolData"/>
      <LatestKg :prData="prData"/>
      <HandPicked :propeuData="propeuData"/>
      <SummerCollection :propelData="propelData"/>
      <BrandKg :propejData="propejData"/>
      <CustomerKg :propeqData="propeqData"/>
    </MainContainer>
  </div>
</template>

<script>
import { propeuData,propelData,propejData,propeqData, prolData,prData } from '../data/data.dummy'

 import ArrivalsKg from '../components/ArrivalsKg.vue'
import BrandKg from '../components/BrandKg.vue'
import HandPicked from '../components/HandPicked.vue'
import SummerCollection from '../components/SummerCollection.vue'
import CustomerKg from '../components/CustomerKg.vue'
import FeaturedArrivals from '../components/FeaturedArrivals.vue'
import LatestKg from '../components/LatestKg.vue'






export default {
  name: 'HomeKg',
  components:{
    FeaturedArrivals,
   ArrivalsKg,
    BrandKg,
    HandPicked,
    SummerCollection,
    CustomerKg,
    LatestKg

  },
  data() {
    return {


      propeuData: propeuData,
      propelData: propelData,
      propejData: propejData,
      propeqData: propeqData,
      prolData: prolData,
      prData: prData,



    }
  }
}
</script>
<style lang="scss" >
</style>