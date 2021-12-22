<template>
  <div class="container q-mb-lg flex justify-between no-wrap">
    <div class="">
      <q-icon class="q-ma-md" :name="icon" size="6rem"/>
    </div>
    <div>
      <h6 class="q-my-sm text-grey-9">{{this.name}}</h6>
      <p class="text-grey-8 text-body1 q-ma-none">{{this.text}}</p>
      <span class="flexbox items-center"><q-icon class="" name="img:img/diamond-sm.png" size="1rem"/>{{this.price}}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'StoreCard',
  props:{
    name: String,
    value: String,
    text: String,
    icon: String,
    price: String,
    size: Number
  }

}
</script>

<style scoped>
  .container {
    border-style: solid;
    border-color: rgb(224, 224, 224);
    border-width: 0.18rem;
    border-radius: 1.4em;
  }
  /* .title {
    font-weight: 800;
  } */
  h6 {
    font-weight: 800;
  }
  span { 
    font-weight: 800;
    color: rgb(28, 176, 246);
  }
</style>