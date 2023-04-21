<template>
    <button class = 'btn'>
        <slot></slot>
    </button>
</template>

<script>
export default {
  name: 'MyButton'
}
</script>

<style scoped>
.btn{
    display: inline-block;
    vertical-align: top;
    text-align: center;

    background-color:rgba(0,0,0,0);
    border: 0;
    padding: 0 25px;
    height: 40px;
    border-right: #404040 solid 1px;

    cursor: pointer;
}
.btn--journal{
  padding: 0 25px 0 50px;
  border: 0;
}
.btn--right{
  border: 0;
  border-left: #404040 solid 1px;
}
.btn--collection{
  border: 0;
}
.btn--mobile{
  display: none;
}

@media (max-width: 1240px) {
  .btn{
    padding: 0px 15px 0px 15px;
  }
}

@media (max-width: 900px){
  .btn{
    display: none;
    padding: 0px 20px 0px 20px;
  }
  .btn--mobile{
    display: inline-block;
  }
  .btn--mobile--logo{
    display: block;
    border: 0;
  }
}
</style>
