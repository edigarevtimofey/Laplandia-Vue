<template>
  <svg class="mobile__icons">
    <use href="#liked__mobile"></use>
  </svg>
  <svg class="svg">
    <symbol id="liked__mobile" viewBox="0 0 17 17">
      <path d="M8.5 15.2847L9.33245 14.4331L9.34315 14.4222L9.3545 14.4119C11.5727 12.4044 13.3676 10.7584 14.6127 9.20858C15.8519 7.66625 16.5 6.27486 16.5 4.78261C16.5 2.35231 14.6732 0.5 12.325 0.5C11.0337 0.5 9.72834 1.12549 8.88529 2.14476L8.5 2.61058L8.11471 2.14476C7.27166 1.12549 5.96625 0.5 4.675 0.5C2.32681 0.5 0.5 2.35231 0.5 4.78261C0.5 6.27486 1.14814 7.66625 2.38728 9.20858C3.63243 10.7584 5.42727 12.4044 7.6455 14.4119L7.65685 14.4222L7.66755 14.4331L8.5 15.2847Z" stroke="#F8F8F8"/>
    </symbol>
  </svg>
</template>

<script>
export default {
  name: 'MyMobileLiked'
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
