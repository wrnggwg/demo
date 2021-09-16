<template>
  <div class="m-floor">
    <div class="header">
      <h2>进口酒饮粮油</h2>
    </div>
    <div class="content">
      <div class="goods">
        <div class="list">
          <a href="javascript:;" class="listItem" v-for="item in info" :key="item">
            <div class="wrap">
              <img src="../../assets/products1.jpg" alt="">
              <h3 class="synopsis">【原装进口，淡淡果香】</h3>
              <p class="from">西班牙进口</p>
              <p class="price">
                <i class="yen">￥</i>
                <span class="priceNum">118</span>
              </p>
              <button class="addShopcar" @click="addShopcar()"></button>
            </div>
          </a>
        </div>
      </div>
      <div class="recommend">
        <div class="words">
          <a href="javascript:;" class="outer" v-for="item in list" :key="item">
            <span class="inner">
              <b class="text">其他食用油</b>
            </span>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods:{
    addShopcar(){
      console.log("a");
    }
  },
  data(){
    return{
      info:[1,2,3,4,5,6,7,8],
      list:[1,2,3,4,5,6,7,8,9]
    }
  }
}
</script>

<style scoped>
.m-floor{
  width: 1190px;
  height: 600px;
}
.header{
  width: 1190px;
  height: 40px;
}
.header h2{
  font-size: 20px;
}
.content{
  position: relative;
  width: 1190px;
  height: 556px;
  border-top: 2px solid black;
}
.goods{
  width: 100%;
  height: 100%;
}
.list{
  width: 798px;
  height: 556px;
  margin-left: 240px;
  margin-right: 150px;
  border: 1px solid #9999;
}
.listItem{
  display: inline-block;
  width: 198px;
  height: 278px;
  text-decoration: none;
}
.wrap{
  position: relative;
  margin: 20px;
  width: 160px;
  height: 250px;
}
.wrap img{
  display: block;
  width: 160px;
  height: 160px;
  margin: 0 auto 10px;
}
.synopsis{
  width: 160px;
  height: 18px;
  font-size: 14px;
  color: black;
}
.from{
  font-size: 12px;
  color: black;
}
.price{
  display: inline;
  margin-top: 20px;
  padding-bottom: 10px;
  width: 75px;
}
.yen{
  font-size: 10px;
  color: black;
}
.priceNum{
  color: black;
}
.addShopcar{
  display: inline;
  margin-left: 70px;
  width: 40px;
  height: 40px;
  border: 0;
  border-radius: 20px;
}
.recommend{
  position: absolute;
  top:0;
  width: 240px;
  height: 260px;
  background: #b373fb;
}
.words{
  padding: 30px 0 30px 20px;
  width: 220px;
  height: 200px;
}
.outer{
  display: inline-block;
  margin: 0 10px 10px 0;
  width: 57px;
  height: 57px;
  border: 1px solid #b373fb;
}
.inner{
  display: inline-block;
  padding: 10px 9px;
  width: 39px;
  height: 37px;
  background: white;
  border-radius: 40px;
}
.text{
  display: inline-block;
  width: 40px;
  height: 28px;
  font-size: 12px;
  font-weight: 400;
  color: black;
  text-align: center;
}
</style>