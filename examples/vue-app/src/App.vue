<script>
import { defineComponent } from 'vue';
import NoBeeHouse from 'nobeehouse-momentodevida-plugin';
import 'nobeehouse-momentodevida-plugin/dist/nobeehouse.min.css';

export default defineComponent({
  mounted() {
    this.plugin = new NoBeeHouse({ el: '#plugin', seePlaces() {} });
  },
  data:() => ({
    plugin: null
  }),
  methods: {
    openPlugin() {
      this.plugin.open();
    }
  }
})
</script>

<template>
  <main class="flex items-center justify-center flex-col h-screen">
    <img src="https://app-30863.nuvem-brasil-10.absamcloud.com/api/public/images/logo-icon.png" alt="Logo NoBeeHouse"
      class="w-64 mb-8" />

    <div>
      <div id="plugin"></div>

      <button id="btn-exemplo"
        class="bg-yellow-500 hover:bg-yellow-400 active:shadow-inner text-white shadow-md px-5 py-3 rounded"
        @click="openPlugin">Ver exemplo</button>
    </div>
  </main>
</template>