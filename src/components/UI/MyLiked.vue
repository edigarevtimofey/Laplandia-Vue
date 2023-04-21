<template>
  <svg class="liked">
    <use xlink:href="#like"></use>
  </svg>
  <svg class="svg">
    <symbol id="like" viewbox="0 0 15 15">
      <g>
        <path d="M7.5 13.2878L8.19391 12.5838L8.20466 12.5729L8.21604 12.5627C10.1743 10.8052 11.754 9.3683 12.849 8.01677C13.9381 6.67253 14.5 5.46916 14.5 4.18478C14.5 2.09542 12.9171 0.5 10.875 0.5C9.75215 0.5 8.61646 1.03987 7.88397 1.91808L7.5 2.37845L7.11603 1.91808C6.38354 1.03987 5.24785 0.5 4.125 0.5C2.0829 0.5 0.5 2.09542 0.5 4.18478C0.5 5.46916 1.06192 6.67253 2.151 8.01677C3.24597 9.3683 4.82566 10.8052 6.78395 12.5627L6.79534 12.5729L6.80609 12.5838L7.5 13.2878Z" stroke="#F8F8F8"/>
      </g>
    </symbol>
  </svg>
</template>

<script>
export default {
  name: 'MyLiked'
}
</script>

<style scoped>
.liked{
    width: 15px;
    height: 15px;
    margin-right: 20px;
}
.svg{
  display: none;
}
@media (max-width: 1240px){
  .liked{
    margin-right: 10px;
  }
}
</style>
