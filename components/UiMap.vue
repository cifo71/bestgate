<template>
<GmapMap
  :center="{lat:48.520195, lng:17.521349}"
  :zoom="12"
  map-type-id="terrain"
  style="width: 1920px; height: 300px"
>
  <GmapMarker
    :key="index"
    :position="{lat:48.520195, lng:17.521349}"
    :clickable="true"
    :draggable="true"
    
  />
</GmapMap>
</template>

<script>
  export default {}
</script>
