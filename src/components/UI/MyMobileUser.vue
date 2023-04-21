<template>
  <svg class="mobile__icons">
    <use href="#user"></use>
  </svg>
  <svg class="svg">
    <symbol id="user" viewbox="0 0 17 17">
      <circle cx="8.5" cy="4.5" r="4" stroke="#F8F8F8"/>
      <path d="M1 16C2.61238 12.9863 5.36954 11 8.5 11C11.6305 11 14.3876 12.9863 16 16" stroke="#F8F8F8"/>
    </symbol>
  </svg>
</template>

<script>
export default {
  name: 'MyMobileUser'
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
