<template>
  <div class="part">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'MyMobileHalfHalf'
}
</script>

<style scoped>
.part{
  display: flex;
  width: 50%;
  height: 40px;
}
.part--left{
  justify-content: left;
}
.part--right{
  justify-content: right;
}
</style>
