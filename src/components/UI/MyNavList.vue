<template>
  <div class="nav__mobile" v-if="showNav">
    <div class="nav__mobile__inner">
      <button class="btn__mobileNav">
        <p class="btn__text__mobileNav">Для неё</p>
      </button>
      <button class="btn__mobileNav">
        <p class="btn__text__mobileNav">Для него</p>
      </button>
      <button class="btn__mobileNav">
        <p class="btn__text__mobileNav">Коллекции</p>
      </button>
      <button class="btn__mobileNav">
        <p class="btn__text__mobileNav">Журнал</p>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyNavList',
  props: {
    showNav: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style scoped>
.nav__mobile{
    display: flex;
    width: 35%;
    height: 132px;
    background-color: #080808;
    border: 0;
}
.nav__mobile__inner{
  display: flex;
  flex-wrap: wrap;
  align-items: center;
}
.btn__mobileNav{
  display: inline-block;
  vertical-align: top;
  text-align: center;

  background-color:rgba(0, 0, 0, 0);
  border: 0;

  cursor: pointer;
  width: 100%;
  height: 20px;
  margin: 5px 15px;
}
.btn__text__mobileNav{
  margin: 0;
  font-family: 'Arial';
  font-style: normal;
  font-weight: 300;
  line-height: 13px;

  letter-spacing: 1px;
  text-transform: uppercase;
  color: #F8F8F8;
  width: 100%;
  font-size: 12px;
  display: flex;
  justify-content: left;
}
</style>
