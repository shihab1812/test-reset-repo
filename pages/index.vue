<template>
  <div id="index-route">
    <nuxt-link to="/menu">GO TO MENU</nuxt-link>
    <div class="card-list-holder">
      <div class="merchant-cards-wrp" v-for="merchantInfo in merchantsInfo" :key="merchantInfo.id">
         <merchant-basic-info-card :data-accept-input="merchantInfo">
         </merchant-basic-info-card>
      </div>
    </div>
  </div>
</template>

<script>
import MerchantBasicInfoCard from '../components/MerchantBasicInfoCard';

export default {
  components: {
    MerchantBasicInfoCard
  },
  created() {
 // call the axios
  },
  data() {
    return{
      test : "shihab",
      merchantsInfo : [{
        id : 1,
        name : "Directi cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img     : 'https://placehold.it/100X100'
      },
      {
        id : 2,
        name : "EGL cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 3,
        name : "Test cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 4,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 5,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 6,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 7,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 8,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 9,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/150X100"
      },
            {
        id : 10,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 11,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 12,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/180X180"
      },
      {
        id : 13,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 14,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 15,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 16,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 17,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 18,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 19,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 20,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 21,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 22,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 23,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 24,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/200X100"
      },
      {
        id : 25,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 26,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 27,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 28,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 29,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 30,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 31,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 32,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 33,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
            {
        id : 34,
        name : "Test4 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },
      {
        id : 35,
        name : "Test2 cafe",
        description : "North Indian, Chinese, south Indian",
        rating      : "4.2",
        img         : "https://placehold.it/100X100"
      },

      ]
    }
  }
}
</script>

<style scoped>
  .card-list-holder .three-row-two-sec-card{
    margin: 10px auto;
  }
</style>
