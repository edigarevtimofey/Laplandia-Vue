<template>
  <svg class="search">
    <use href="#search"></use>
  </svg>
  <svg class="search search--mobile">
    <use href="#search__mobile"></use>
  </svg>

  <svg class="svg">
    <symbol id="search" viewbox="0 0 17 17">
    <g>
      <path d="M0.555573 0.555555L5.00002 5" stroke="#F8F8F8"/>
      <circle cx="7.11111" cy="7.11111" r="6.61111" stroke="#F8F8F8"/>
    </g>
    </symbol>
  </svg>
  <svg class="svg">
    <symbol id="search__mobile" viewbox="0 0 17 17">
    <g>
      <circle cx="6.5" cy="6.5" r="6" stroke="#F8F8F8"/>
      <path d="M11 11L16 16" stroke="#F8F8F8"/>
    </g>
    </symbol>
  </svg>
</template>

<script>
export default {
  name: 'MySearch'
}
</script>

<style scoped>
.search{
    width: 15px;
    height: 15px;
    transform: scale(-1, -1);
}
.search--mobile{
    width: 20px;
    height: 20px;
    transform: scale(1, 1);
    align-content: center;
    justify-content: center;
    display: none;
    flex-wrap: wrap;
}
.svg{
  display: none;
}
@media (max-width: 900px){
  .search{
    display: none;
  }
  .search--mobile{
    display: flex;
  }
}
</style>
