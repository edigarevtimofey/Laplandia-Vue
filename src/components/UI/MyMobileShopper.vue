<template>
  <svg class="mobile__icons">
    <use href="#shopper"></use>
  </svg>
  <svg class="svg">
    <symbol id="shopper" viewbox="0 0 17 17">
      <path d="M3 7C4.07492 2.32638 5.91303 1 8 1C10.087 1 11.9251 2.32638 13 7" stroke="#F8F8F8"/>
      <rect x="0.5" y="7.5" width="15" height="9" stroke="#F8F8F8"/>
    </symbol>
  </svg>
</template>

<script>
export default {
  name: 'MyMobileShopper'
}
</script>

<style scoped>
.mobile__icons{
    width: 17px;
    height: 17px;
    display: none;
}
.svg{
  display: none;
}
@media (max-width: 900px){
  .mobile__icons{
    display: block;
  }
}
</style>
