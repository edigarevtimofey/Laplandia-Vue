<template>
  <div class="half__header">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'MyMobileHalf'
}
</script>

<style scoped>
.half__header{
  height: 40px;
  width: 100%;
  display: none;
  align-content: center;
  justify-content: center;
  border-bottom: 1px solid #404040;

}
@media (max-width: 900px){
  .half__header{
    display: flex;
    flex-wrap: wrap;
  }
}
</style>
