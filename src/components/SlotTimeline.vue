<script>
import { ref } from 'vue'
import * as renderjson from 'renderjson'
import CollapsibleJson from './CollapsibleJson.vue'


export default {
  props: {
    msg: String,
    jsonData: {
      type: Object,
      // Object or array defaults must be returned from
      // a factory function. The function receives the raw
      // props received by the component as the argument.
      default(rawProps) {
        return {}
      }
    }
  },
  components: {
    'collapsible-json': CollapsibleJson,
  },
  data() {
    return {
    }
  },

  mounted() {
  }
}
</script>

<template>
    <v-timeline direction="horizontal" align="start" side="end">
      <template v-for="val, key in jsonData.pcap.ad_details">
        <collapsible-json :data=val :id=key>
        </collapsible-json>
      </template>
    </v-timeline>
</template>

<style>
</style>

