<template>
  <div id="cesiumContainer"></div>
</template>

<script>
import { onMounted } from "vue";
import useViewer from "@/hooks/useViewer"


export default {
  name: "CesiumViewer",
  setup() {
    onMounted(() => {
      useViewer();
      
    });
  },
};
</script>
<style>
html,
body,
#cesiumContainer {
  height: 100%;
  width: 100%;
  margin: 0;
  padding: 0;
  overflow: hidden;
}
</style>
