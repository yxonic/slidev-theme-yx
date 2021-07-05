<template>
  <div class="slidev-layout grid grid-cols-2 gap-12 w-full h-full">
    <div class="">
      <slot />
    </div>

    <div class="">
      <img :src="image" alt="" class="w-full h-full object-cover rounded-lg" />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    image: {
      type: String,
      required: false,
    },
  },
})
</script>
