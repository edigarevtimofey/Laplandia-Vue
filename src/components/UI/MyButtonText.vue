<template>
    <div class="btn__text">
        <slot></slot>
    </div>
</template>

<script>
export default {
  name: 'MyButtonText'
}
</script>

<style scoped>
.btn__text{
    margin: 0;
    font-family: 'Arial';
    font-style: normal;
    font-weight: 700;
    font-size: 11px;
    line-height: 13px;

    letter-spacing: 1px;
    text-transform: uppercase;
    color: #F8F8F8;
}
.btn__text--mg{
  margin-right: 15px;
}
.btn__text--mgl{
  margin-left: 15px;
}
.btn__text--big{
  font-size: 14px !important;
}
@media (max-width: 1240px){
    .btn__text{
        font-size: 10px;
    }
    .btn__text--mg{
      margin-right: 10px;
    }
  }
  @media (max-width: 1040px){
    .btn__text{
      font-size: 9.5px;
    }
  }
</style>
