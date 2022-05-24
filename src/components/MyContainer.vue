<template>
<div class="container">
  <slot></slot>
</div>
</template>

<script>
export default {
  name: "MyContainer.vue"
}
</script>

<style scoped>
.container{
  display: flex;
  width: 100%;
}
</style>