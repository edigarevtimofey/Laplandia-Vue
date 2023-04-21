<template>
  <div class="burger" type="button">
    <span class="burger__item">Menu</span>
  </div>
</template>

<script>
export default {
  name: 'MyBurger'
}
</script>

<style scoped>
.burger{
    display: none;
    background: none;
    border: 0;
    cursor: pointer;
    padding: 9px 2px;
}
.burger__item{
    display: block;
    width: 30px;
    height: 0.5px;

    background-color: #fff;

    font-size: 0;
    color: transparent;

    position: relative;
}
.burger__item:before,
.burger__item:after{
    content: "";
    width: 100%;
    height: 100%;
    background-color: #fff;

    position: absolute;
    left: 0;
    z-index: 1;
}
.burger__item:before{
    top: -8px;
}
.burger__item:after{
    bottom: -8px;

}
@media (max-width: 900px){
  .burger{
    display: block;
  }
}
</style>
