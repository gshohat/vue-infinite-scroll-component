<script setup>

const props = defineProps(['options']);
const items = await props.options.fetchData()

</script>


<template>

  <div class="scrollbar">
    <slot :items="items"></slot>
  </div>

</template>

<style scoped>

.scrollbar {
  overflow: scroll;
  height: 90%;
}

</style>

