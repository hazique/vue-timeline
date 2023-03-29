<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <v-timeline direction="horizontal" align="start" truncate-line="end">
    <v-timeline-item>
      <div>
        <div class="text-h6">Content title</div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
      </div>
    </v-timeline-item>

    <v-timeline-item>
      <div>
        <div class="text-h6">Content title</div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
      </div>
    </v-timeline-item>

    <v-timeline-item>
      <div>
        <div class="text-h6">Content title</div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
      </div>
    </v-timeline-item>
  </v-timeline>
</template>

<style>
.v-timeline-divider{
  width: 120%;
}
</style>

