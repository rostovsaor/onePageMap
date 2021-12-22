<template>
  <q-page class="q-ma-lg">
    <div class="flexbox row justify-between">
      <div>
        <h4 class="q-ma-none" style="font-weight: 800;">Salvador Rombe</h4>
        <p class="q-ma-none text-subtitle2 text-grey-7">SalvadorRo7751</p>
        <p class="q-ma-none text-grey-7"><q-icon class="q-ml-none q-mr-sm" name="timer" />Por aqui desde agosto de 2020</p>
      </div>
      <div class="bg-grey-9 q-pl-lg" style="border-radius:2em; font-size:5em; width: 1.4em; color: white; ">S</div>
    </div>

    <q-separator></q-separator>
    <h5>Estatisticas</h5>



    <StoreCard 
      name="Bloqueio de ofensiva" 
      price="Dias de ofensiva" 
      text="0." 
      icon="img:img/streak-freeze.svg"
      size="2"
    />
    <StoreCard 
      name="Aposta: O Dobro ou Nada" 
      price="50" 
      text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais" 
      icon="img:img/flaming-calendar.svg"
    />

    <h5>Cristais</h5>
    <StoreCard 
      name="Bloqueio de ofensiva" 
      price="200" 
      text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez." 
      icon="img:img/streak-freeze.svg"
    />
    <StoreCard 
      name="Aposta: O Dobro ou Nada" 
      price="50" 
      text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais" 
      icon="img:img/flaming-calendar.svg"
    />

    <h5>Vidas</h5>
    <StoreCard 
      name="Bloqueio de ofensiva" 
      price="200" 
      text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez." 
      icon="img:img/streak-freeze.svg"
    />
    <StoreCard 
      name="Aposta: O Dobro ou Nada" 
      price="50" 
      text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais" 
      icon="img:img/flaming-calendar.svg"
    />

    <h5>Trajes</h5>
    <StoreCard 
      name="Bloqueio de ofensiva" 
      price="200" 
      text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez." 
      icon="img:img/streak-freeze.svg"
    />
    <StoreCard 
      name="Aposta: O Dobro ou Nada" 
      price="50" 
      text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais" 
      icon="img:img/flaming-calendar.svg"
    />
  </q-page>
</template>

<script>
    // import BigNewsComponent from "../items-component/BigNewsComponent";

import StoreCard from "components/maza/StoreCard.vue"
export default {
  name: 'Profile',
  components: {
    StoreCard
  }
}
</script>

<style>
  h4, h5 {
    font-weight: 800;
    color:rgb(80, 80, 80);
    margin: 3rem 0 1rem 0;

  }
  .container {
    border-style: solid;
    border-color: rgb(224, 224, 224);
    border-width: 0.18rem;
    border-radius: 1.4em;
  }
</style>