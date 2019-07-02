<template>
    <ul class="nav">
      <li class='logo-img'>
        <img src='' >
      </li>
      <li class="nav-item" v-for="(item,index) in navs" :key="index">
        <a :href="item.address" class="nav-btn">{{item.name}}</a>
      </li>
      <li class='avatar-img'>
        <img src='' >
      </li>   
    </ul>
</template>

<script>
export default {
  data() {
    return {
      isOpacity: false,
      navs:[
        {address:"",name:"主页"},
        {address:"",name:"关于"},
        {address:"",name:"常见问题"}
      ]
    }
  },
  mounted () {

  },
  methods: {

  }
}
</script>

<style lang="scss" scoped>

  .nav {
    display: flex;
    justify-content: flex-end;
    width: 100%;
    position: fixed;
    height: 80px;
    line-height: 60px;
    background-color: rgba(255, 255, 255, .8);
    z-index: 100;
    transition: all 1s ease;
    padding: 10px 30px;
    .logo-img{
      position: absolute;
      width: 180px;
      height: 60px;
      left: 30px;
      margin:0;
      padding: 0;
      background: green;
    }
    .nav-item{
      display: inline-block;
      width: 80px;
      height: 60px;
      }
    .nav-btn{
      display: inline-block;
      }
    .avatar-img{
        width: 40px;
        height: 40px;
        margin:10px;
        padding: 0;
        border-radius: 20px;
        background: red;
      }
    }

</style>
