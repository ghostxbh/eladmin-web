<template>
  <elFrame :src="drawingApi" />
</template>
<script>
import { mapGetters } from 'vuex'
import elFrame from '@/components/Iframe/index'
export default {
  name: 'Drawing',
  components: { elFrame },
  computed: {
    ...mapGetters([
      'drawingApi'
    ])
  }
}
</script>
