<template>
  <div class="nav">
    <router-link class="item" to="/money" active-class="selected">
      <Icon name = 'money'></Icon>
      记账
    </router-link>
    <router-link class="item" to="/labels"  active-class="selected">
      <Icon name = 'label'></Icon>
      标签
    </router-link>
    <router-link class="item" to="/statistics"  active-class="selected">
       <Icon name = 'tongji'></Icon>
      统计
    </router-link>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@keyframes on {
  from{
   transform: rotate(0deg);
  }
  to{
    transform: rotate(360deg);
  }
}
.nav {
  font-size: 12px;
  display: flex;
  box-shadow: 0 0 3px rgba(0,0,0,0.25);
  flex-direction: row;
  > .item{
    width: 33.3333%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    .icon {
      width: 32px;
      height: 32px;
    }
  }
  > .item.selected {
    color: red;
  }
  > .item:first-child.selected .icon{
     animation: on .7s linear
  }
}
</style>