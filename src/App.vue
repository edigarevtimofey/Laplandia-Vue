<template>
  <div class="header">
    <div class="header__inner">
      <div>
        <MyButton>
          <MyButtonText>
            для неё
          </MyButtonText>
        </MyButton>
        <MyButton>
          <MyButtonText>
            для него
          </MyButtonText>
        </MyButton>
        <MyButton class="btn btn--collection">
          <MyButtonText>
            коллекции
          </MyButtonText>
        </MyButton>
        <MyButton class="btn btn--journal">
          <MyButtonText>
            журнал
          </MyButtonText>
        </MyButton>
      </div>
      <div class="logo">
        <MyButton class="btn btn--collection">
          <MyLogo></MyLogo>
        </MyButton>
      </div>
      <div>
        <MyButton class="btn btn--right btn--collection">
          <div class="flex">
            <MyLiked></MyLiked>
            <MyButtonText>
              0
            </MyButtonText>
          </div>
        </MyButton>
        <MyButton class="btn btn--right">
          <MySearch></MySearch>
        </MyButton>
        <MyButton class="btn btn--right">
          <MyButtonText>
            мой аккаунт
          </MyButtonText>
        </MyButton>
        <MyButton class="btn btn--right">
          <div class="flex">
            <MyButtonText class="btn__text btn__text--mg">
              корзина
            </MyButtonText>
            <MyButtonText>
              0
            </MyButtonText>
          </div>
        </MyButton>
      </div>
    </div>
  <div class="mobile__inner">
    <MyMobileHalf>
      <div class="logo">
        <MyButton class="btn btn--mobile--logo">
          <MyLogo></MyLogo>
        </MyButton>
      </div>
    </MyMobileHalf>
    <MyMobileHalf>
      <MyMobileHalfHalf class="part part--left">
        <MyButton class="btn btn--mobile btn--collection" @click="showNav">
          <MyBurger></MyBurger>
        </MyButton>
        <MyButton class="btn btn--mobile btn--collection">
          <MySearch></MySearch>
        </MyButton>
      </MyMobileHalfHalf>
      <MyMobileHalfHalf class="part part--right">
        <MyButton class="btn btn--mobile btn--right">
          <div class="flex">
            <MyMobileLiked></MyMobileLiked>
            <MyButtonText class="btn__text btn__text--big btn__text--mgl">0</MyButtonText>
          </div>
        </MyButton>
        <MyButton class="btn btn--mobile">
          <div class="flex">
            <MyMobileShopper></MyMobileShopper>
            <MyButtonText class="btn__text btn__text--big btn__text--mgl">0</MyButtonText>
          </div>
        </MyButton>
        <MyButton class="btn btn--mobile btn--collection">
          <MyMobileUser></MyMobileUser>
        </MyButton>
      </MyMobileHalfHalf>
    </MyMobileHalf>
    <MyNavList v-model:showNav="NavVisible">
    </MyNavList>
  </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      NavVisible: false
    }
  },
  methods: {
    showNav () {
      if (this.NavVisible) {
        this.NavVisible = false
      } else {
        this.NavVisible = true
      }
    }
  }
}
</script>

<style scoped>
.logo{
  display: flex;
  align-content: center;
   justify-content: center;
}
.header{
    display: flex;
    position: absolute;
    left: 0%;
    right: 0%;
    top: 0%;
    bottom: 0%;
    height: 40px;
    background: #080808;
    border-bottom: 1px solid #404040;

    font-family: Arial, Helvetica, sans-serif;
}
.header__inner{
    background-color: #080808;
    width: 100%;

    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    justify-content: center;
    align-items: center;

}
.flex{
  display: flex;
  flex-wrap: wrap;
  align-items: center;
}
.mobile__inner{
  display: none;
  flex-wrap: wrap;
  width: 100%;
}
@media (max-width: 900px){
  .header{
    height: 80.5px;
  }
  .header__inner{
    display: none;
  }
  .mobile__inner{
    display: flex;
  }
}
</style>
