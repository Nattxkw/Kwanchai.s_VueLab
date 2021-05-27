<template>
  <div class="container">
    <manufacturer v-slot="data">
      <devices :manufacturerId="data.factId"></devices>
    </manufacturer>
  </div>
</template>

<script>
import Manufacturer from "@/components/Manufacturer.vue"; //@บอกว่าอยู่ในsrc
import Devices from "@/components/Devices.vue";
export default {
  components: {
    Manufacturer: Manufacturer,
    Devices: Devices,
  },
};
</script>