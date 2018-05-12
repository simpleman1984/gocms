<template>
  <pano title="The Title" width="720" height="480" bundle="assets/logo/" format="jpg"></pano>
</template>
<script>
  import pano from 'vue-pano'

  export default {
    components: {
      pano
    }
  }
</script>
