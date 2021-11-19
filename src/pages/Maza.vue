<template>
  <div class="q-ma-lg">
    <h5>Ofensiva</h5>
    <StoreCard name="Bloqueio de ofensiva" value="200" text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez." icon="img/"/>
    <StoreCard name="Aposta: O Dobro ou Nada" value="50" text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais"/>

    <h5>Cristais</h5>
    <StoreCard name="Bloqueio de ofensiva" value="200" text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez."/>
    <StoreCard name="Aposta: O Dobro ou Nada" value="50" text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais"/>

    <h5>Vidas</h5>
    <StoreCard name="Bloqueio de ofensiva" value="200" text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez."/>
    <StoreCard name="Aposta: O Dobro ou Nada" value="50" text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais"/>

    <h5>Trajes</h5>
    <StoreCard name="Bloqueio de ofensiva" value="200" text="Proteja a sua ofensiva se perder um dia de prática. Coloque até 2 em uso de umma vez."/>
    <StoreCard name="Aposta: O Dobro ou Nada" value="50" text="Mantenha 7 dias de ofensiva pra dobrar a sua aposta de 50 cristais"/>
  </div>
</template>

<script>
    // import BigNewsComponent from "../items-component/BigNewsComponent";

import StoreCard from "components/maza/StoreCard.vue"
export default {
  name: 'Maza',
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
</style>