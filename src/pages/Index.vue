<template>
  <q-page class="flex flex-center">
    <l-map style="height:95vh" ref="map" v-model:zoom="zoom" :center="mozCenter" @click="click">
      <l-tile-layer
        url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png"
        layer-type="base"
        name="OpenStreetMap"
      ></l-tile-layer>
      <l-circle 
        v-for="item in provData" 
        :key="item.name" 
        :lat-lng="item.latlng" 
        :radius="item.radius"
        color="green"
        fillColor="#e4ce7f"
        fillOpacity: 1
      >
        <l-popup>
          <p><b>{{item.name}}</b></p>
          <b>Nº de Clientes:</b> {{item.radius}}
        </l-popup>
      </l-circle>
    </l-map>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';
import "leaflet/dist/leaflet.css"
import { LMap, LGeoJson, LTileLayer, LCircle, LPopup, LCircleMarker } from "@vue-leaflet/vue-leaflet";


export default defineComponent({
  name: 'PageIndex',
  components: {
    LMap,
    LGeoJson,
    LTileLayer,
    LCircle,
    LPopup,
    LCircleMarker
  },
  setup() {
    return {
      zoom: 6,
      mozCenter:[-19.4514005, 34.05761718],
      provData:[
        {
          name: 'Maputo',
          latlng: [-25.71647, 32.21191],
          radius: 95000
        },
        {
          name: 'Gaza',
          latlng: [-23.53974, 32.71728],
          radius: 75000
        },
        {
          name: 'Inhambane',
          latlng: [-23.03465, 34.56298],
          radius: 60000
        },
        {
          name: 'Manica',
          latlng: [-18.99523, 33.26660],
          radius: 55000
        },
        {
          name: 'Sofala',
          latlng: [-19.30661, 34.49707],
          radius: 65000
        },
        {
          name: 'Tete',
          latlng: [-15.40562, 32.78320],
          radius:50000
        },
        {
          name: 'Zambezia',
          latlng: [-16.73655, 36.80419],
          radius:45000
        },
        {
          name: 'Nampula',
          latlng: [-15.02459, 39.26513],
          radius:65000
        },
        {
          name: 'Niassa',
          latlng: [-13.17043, 36.47460],
          radius:25000
        },
        {
          name: 'Cabo Delgado',
          latlng: [-12.52769, 39.33105],
          radius:45000
        },
      ]

    };
  },
  methods: {
    getRandomInt: function(min, max) {
      min = Math.ceil(min);
      max = Math.floor(max);
      return Math.floor(Math.random() * (max - min) + min); //The maximum is exclusive and the minimum is inclusive
    },
    click(e) {
      console.log("event :", e)
    }
  },
  async beforeMount() {
    // // HERE is where to load Leaflet components!
    // const { circleMarker } = await import("leaflet/dist/leaflet-src.esm");

    // // And now the Leaflet circleMarker function can be used by the options:
    // this.geojsonOptions.pointToLayer = (feature, latLng) =>
    //   circleMarker(latLng, { radius: 8 });
    // this.mapIsReady = true;
  },
})
</script>
