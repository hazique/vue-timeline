<script >
import SlotTimeline from './components/SlotTimeline.vue'
import data from './assets/data.json'
import { ref } from 'vue';

export default {
  components: {
    SlotTimeline
  },

  data(){
    return {
      data: ref(data)
    }
  },
  mounted(){
  }
}
</script>

<template>
  <SlotTimeline :jsonData=data msg="Test Message"></SlotTimeline>
</template>

<style>

</style>

