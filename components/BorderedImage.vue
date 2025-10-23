<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps({
    imgPath: {
    default: "",
  },
  customWidth: {
    default: "",
  },
})

const imgPath = ref(props.imgPath);
const customWidth = ref(props.customWidth)
</script>

<template>
    <img :src="imgPath" :width="customWidth" />
</template>

<style scoped>
img {
  border: 1px solid black;
  margin: 0 auto;
}
</style>