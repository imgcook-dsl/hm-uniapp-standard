<template>
  <div class="box">
    <div class="hd">
      <div class="block">
        <span class="txt">收银</span>
        <div class="group">
          <img class="iconTest" :src="constants.image1" />
          <span class="text">交接班</span>
        </div>
      </div>
      <div class="block_4">
        <div class="block_2">
          <div class="dianhuaWrap">
            <img class="dianhua" :src="constants.image2" />
            <img class="lu" :src="constants.image3" />
            <img class="dot" :src="constants.image4" />
          </div>
          <span class="txt_2">新增会员</span>
        </div>
        <div class="group_2">
          <img class="bianji" :src="constants.image5" />
          <span class="word">商品编辑</span>
        </div>
        <div class="block_3">
          <img class="tulixianshi" :src="constants.image6" />
          <span class="text_2">菜单</span>
        </div>
      </div>
    </div>
    <div class="bd">
      <div class="block_13">
        <div class="color" />
        <div class="group_3">
          <span class="txt_3">牛肉汉堡</span>
          <div class="priceWrap"><span class="price">￥22/份</span></div>
        </div>
        <div class="block_5">
          <span class="word_2">牛肉汉堡</span>
          <div class="moneyWrap"><span class="money">￥22/份</span></div>
        </div>
        <div class="group_4">
          <span class="text_3">薯条</span>
          <div class="priceWrap_2"><span class="price_2">￥18/份</span></div>
        </div>
        <div class="block_6">
          <span class="txt_4">牛肉汉堡</span>
          <div class="moneyWrap_2"><span class="money_2">￥22/份</span></div>
        </div>
        <div class="group_5">
          <span class="word_3">牛肉汉堡</span>
          <div class="priceWrap_3"><span class="price_3">￥22/份</span></div>
        </div>
        <div class="block_7">
          <span class="text_4">牛肉汉堡</span>
          <div class="moneyWrap_3"><span class="money_3">￥22/份</span></div>
        </div>
        <div class="group_6">
          <span class="title">田园鸡腿堡</span>
          <div class="priceWrap_4"><span class="price_4">￥22/份</span></div>
        </div>
        <div class="block_8">
          <span class="word_4">牛肉汉堡</span>
          <div class="moneyWrap_4"><span class="money_4">￥22/份</span></div>
        </div>
        <div class="group_7">
          <span class="text_5">牛肉汉堡</span>
          <div class="priceWrap_5"><span class="price_5">￥22/份</span></div>
        </div>
        <div class="block_9"><div class="colorDiv" /></div>
        <div class="group_8">
          <span class="txt_5">牛肉汉堡</span>
          <div class="moneyWrap_5"><span class="money_5">￥22/份</span></div>
        </div>
        <div class="block_10">
          <span class="word_5">牛肉汉堡</span>
          <div class="priceWrap_6"><span class="price_6">￥22/份</span></div>
        </div>
        <div class="group_9">
          <span class="text_6">麻辣汉堡</span>
          <div class="moneyWrap_6"><span class="money_6">￥22/份</span></div>
        </div>
        <div class="block_11"><div class="color_2" /></div>
        <div class="group_10">
          <span class="txt_6">牛肉汉堡</span>
          <div class="priceWrap_7"><span class="price_7">￥22/份</span></div>
        </div>
        <div class="block_12">
          <span class="title_2">香辣鸡腿堡</span>
          <div class="moneyWrap_7"><span class="money_7">￥26/份</span></div>
        </div>
        <div class="group_11">
          <span class="text_7">小炒</span> <span class="txt_7">主食</span>
          <span class="word_6">面食</span> <span class="text_8">粉类</span>
          <span class="txt_8">汉堡</span> <span class="word_7">意面</span>
          <span class="text_9">饮品</span> <span class="txt_9">套餐</span>
        </div>
        <div class="colorDiv_2" />
      </div>
      <div class="block_18">
        <div class="color_3" />
        <div class="block_14">
          <div class="container">
            <span class="text_10">序号</span> <span class="txt_10">菜品</span>
          </div>
          <span class="word_8">小计</span>
        </div>
        <div class="group_12">
          <div class="tagWrap"><span class="tag">会员登录</span></div>
        </div>
        <div class="priceWrap_8">
          <span class="num">01</span> <span class="desc">香辣鸡腿堡</span>
          <span class="price_8">￥22.00</span>
        </div>
        <div class="empty" />
        <div class="moneyWrap_8">
          <span class="num_2">02</span> <span class="desc_2">香辣鸡腿堡</span>
          <span class="money_8">￥22.00</span>
        </div>
        <div class="div" />
        <div class="priceWrap_9">
          <span class="num_3">03</span> <span class="txt_11">薯条</span>
          <span class="price_9">￥28.00</span>
        </div>
        <span class="word_9">小份</span>
        <div class="empty_2" />
        <div class="group_13">
          <span class="num_4">04</span>
          <span class="desc_3">会员折扣（98折）</span>
          <span class="money_9">-￥10.00</span>
        </div>
        <div class="block_17">
          <div class="grid">
            <div class="col1"><span class="tag_2">备注</span></div>
            <div class="col2"><span class="tag_3">挂单</span></div>
            <div class="col3"><span class="tag_4">清单</span></div>
            <div class="col4"><span class="tag_5">折扣</span></div>
          </div>
          <span class="desc_4">整单备注：多辣、多番茄酱、不要葱花</span>
          <div class="container_2">
            <span class="text_11">总计：123.00</span>
            <div class="priceWrap_10">
              <span class="word_10">应付：</span>
              <span class="price_10">￥113.00</span>
            </div>
          </div>
          <div class="block_16">
            <div class="block_15">
              <img class="weixinzhifu" :src="constants.image7" />
              <span class="txt_12">微信支付</span>
            </div>
            <div class="infoWrap">
              <img class="zhifubao" :src="constants.image8" />
              <span class="info">支付宝支付</span>
            </div>
            <div class="container_3">
              <div class="welcomesvgiconWrap">
                <img class="welcomesvgicon" :src="constants.image9" />
                <img class="Minus" :src="constants.image10" />
                <img class="image" :src="constants.image11" />
                <img class="picture" :src="constants.image12" />
                <img class="verticalLine" :src="constants.image13" />
              </div>
              <span class="text_12">现金支付</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmUniAppDemoComponent',
  props: {
    dataId: {
      type: String,
      default: 'hm-uni-app-demo-component'
    },
    options: {
      type: Object,
      default: function() {
        return {};
      }
    }
  },
  data() {
    return {
      constants: {
        image1:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/058e9c40465811eabc84cf42e4760be1.png',
        image2:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/06841fd0465811ea9b17f9c51ac2386e.png',
        image3:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/06f27200465811ea82a00d7d610ea15e.png',
        image4:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/06b40970465811eaab34216341d38906.png',
        image5:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/05d7b330465811ea8dd5f16f7d7acfdb.png',
        image6:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/072f53f0465811eab5896d6b6f989c88.png',
        image7:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/0437e5e0465811eaadb621dac880eba4.png',
        image8:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/054f2240465811eaada51b80e9c93470.png',
        image9:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/04651060465811ea9f2387760fbedd51.png',
        image10:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/048d0ac0465811eaa41d0f4a2a6bd458.png',
        image11:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/04b86080465811eab768bd6523a52505.png',
        image12:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/04db03b0465811eab30213045b3a7088.png',
        image13:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/051d15c0465811eaa575d708266b0c31.png'
      }
    };
  },
  methods: {}
};
</script>
<style src="./index.response.css" />
