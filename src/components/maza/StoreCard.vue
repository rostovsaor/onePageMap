<template>
  <div class="container q-mb-lg flex justify-between no-wrap">
    <div class="">
      <q-icon class="q-ma-md" name="img:img/ofensiva1.png" size="6rem"/>
    </div>
    <div>
      <h6 class="q-my-sm text-grey-9">{{this.name}}</h6>
      <p class="text-grey-8 text-body1">{{this.text}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'StoreCard',
  props:{
    name: String,
    value: Number,
    text: String,
  }
    // <StoreCard name="Bloqueio de ofensiva" value="200" text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez."/>

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
</style>